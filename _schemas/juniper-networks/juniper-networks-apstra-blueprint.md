---
description: Schema for a Juniper Apstra blueprint object. Blueprints are the central construct in Apstra intent-based networking. A blueprint represents the complete intended state of a data center network fabric, instantiated from a template that defines the leaf-spine topology. The blueprint contains the network graph with nodes (spines, leaves, servers), links, IP addressing, BGP configuration, security zones (VRFs), virtual networks (VLANs/VXLANs), and connectivity templates. Apstra continuously validates the actual network state against the blueprint intent and raises anomalies when deviations are detected. Changes are staged in the blueprint and deployed to devices through a commit/deploy workflow.
layout: schema
name: Juniper Apstra Blueprint
properties_list:
- description: Blueprint unique identifier assigned by the Apstra server upon creation.
  name: id
  type: string
- description: Human-readable blueprint name. Typically identifies the data center or pod the blueprint represents.
  name: label
  type: string
- description: Blueprint design type. Currently supports two_stage_l3clos for leaf-spine (2-stage Clos) data center fabric topologies.
  name: design
  type: string
- description: Blueprint deployment lifecycle status. 'created' indicates initial creation, 'ready' indicates the blueprint is operational and deployed, 'deploying' indicates active configuration push, 'deploy_error
  name: status
  type: string
- description: Blueprint version number. Incremented on each successful commit/deploy operation. Used for optimistic concurrency control.
  name: version
  type: integer
- description: Reference to the template used to instantiate this blueprint. Templates define the topology structure including spine count, rack types, and link speeds.
  name: template_id
  type:
  - string
  - 'null'
- description: Number of build errors in the current blueprint configuration. Build errors indicate configuration conflicts or missing resources that must be resolved before deployment.
  name: build_errors_count
  type: integer
- description: Number of build warnings. Warnings indicate non-critical issues that do not prevent deployment but may affect network behavior.
  name: build_warnings_count
  type: integer
- description: Summary counts of active anomalies by category. Anomalies represent deviations between blueprint intent and actual network state.
  name: anomaly_counts
  type: object
- description: Count of nodes in the blueprint graph by role.
  name: nodes_count
  type: object
- description: Blueprint creation timestamp.
  name: created_at
  type: string
- description: Last blueprint modification timestamp.
  name: last_modified_at
  type: string
provider_name: Juniper Networks
provider_slug: juniper-networks
schema_file: json-schema/juniper-networks-apstra-blueprint-schema.json
slug: juniper-networks-apstra-blueprint
source_filename: juniper-networks-apstra-blueprint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/json-schema/juniper-networks-apstra-blueprint-schema.json\",\n  \"title\": \"Juniper Apstra Blueprint\",\n  \"description\": \"Schema for a Juniper Apstra blueprint object. Blueprints are the central construct in Apstra intent-based networking. A blueprint represents the complete intended state of a data center network fabric, instantiated from a template that defines the leaf-spine topology. The blueprint contains the network graph with nodes (spines, leaves, servers), links, IP addressing, BGP configuration, security zones (VRFs), virtual networks (VLANs/VXLANs), and connectivity templates. Apstra continuously validates the actual network state against the blueprint intent and raises anomalies when deviations are detected. Changes are staged in the blueprint and deployed to devices through a commit/deploy workflow.\"\
  ,\n  \"type\": \"object\",\n  \"required\": [\"label\", \"design\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Blueprint unique identifier assigned by the Apstra server upon creation.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable blueprint name. Typically identifies the data center or pod the blueprint represents.\",\n      \"minLength\": 1,\n      \"maxLength\": 128\n    },\n    \"design\": {\n      \"type\": \"string\",\n      \"enum\": [\"two_stage_l3clos\"],\n      \"description\": \"Blueprint design type. Currently supports two_stage_l3clos for leaf-spine (2-stage Clos) data center fabric topologies.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"created\", \"ready\", \"deploying\", \"deploy_error\"],\n      \"description\": \"Blueprint deployment lifecycle status. 'created' indicates initial creation, 'ready' indicates the\
  \ blueprint is operational and deployed, 'deploying' indicates active configuration push, 'deploy_error' indicates a failed deployment.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Blueprint version number. Incremented on each successful commit/deploy operation. Used for optimistic concurrency control.\",\n      \"minimum\": 0\n    },\n    \"template_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uuid\",\n      \"description\": \"Reference to the template used to instantiate this blueprint. Templates define the topology structure including spine count, rack types, and link speeds.\"\n    },\n    \"build_errors_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of build errors in the current blueprint configuration. Build errors indicate configuration conflicts or missing resources that must be resolved before deployment.\",\n      \"minimum\": 0\n    },\n    \"build_warnings_count\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Number of build warnings. Warnings indicate non-critical issues that do not prevent deployment but may affect network behavior.\",\n      \"minimum\": 0\n    },\n    \"anomaly_counts\": {\n      \"type\": \"object\",\n      \"description\": \"Summary counts of active anomalies by category. Anomalies represent deviations between blueprint intent and actual network state.\",\n      \"properties\": {\n        \"total\": {\n          \"type\": \"integer\",\n          \"description\": \"Total active anomaly count across all categories.\"\n        },\n        \"config\": {\n          \"type\": \"integer\",\n          \"description\": \"Configuration deviation anomalies.\"\n        },\n        \"cabling\": {\n          \"type\": \"integer\",\n          \"description\": \"Physical cabling mismatch anomalies.\"\n        },\n        \"bgp\": {\n          \"type\": \"integer\",\n          \"description\": \"BGP session state anomalies.\"\n        },\n    \
  \    \"interface\": {\n          \"type\": \"integer\",\n          \"description\": \"Interface state anomalies.\"\n        },\n        \"route\": {\n          \"type\": \"integer\",\n          \"description\": \"Routing table anomalies.\"\n        },\n        \"liveness\": {\n          \"type\": \"integer\",\n          \"description\": \"Device liveness (unreachable) anomalies.\"\n        }\n      }\n    },\n    \"nodes_count\": {\n      \"type\": \"object\",\n      \"description\": \"Count of nodes in the blueprint graph by role.\",\n      \"properties\": {\n        \"spine\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of spine switches.\"\n        },\n        \"leaf\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of leaf switches.\"\n        },\n        \"access\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of access switches.\"\n        },\n        \"generic\": {\n          \"type\": \"integer\"\
  ,\n          \"description\": \"Number of generic systems (servers, storage).\"\n        },\n        \"external_router\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of external routers connected to the fabric.\"\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Blueprint creation timestamp.\"\n    },\n    \"last_modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last blueprint modification timestamp.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/json-schema/juniper-networks-apstra-blueprint-schema.json
tags:
- Automation
- Cloud
- Data Center
- Enterprise
- Networking
- SDN
- Security
title: Juniper Apstra Blueprint
---
