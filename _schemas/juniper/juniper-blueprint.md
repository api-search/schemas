---
description: Schema representing a Juniper Apstra data center blueprint. A blueprint is the core abstraction in Apstra that defines the intended state of a data center fabric, including its topology, resource allocations, virtual networks, and policies.
layout: schema
name: Juniper Apstra Blueprint
properties_list:
- description: Unique blueprint identifier
  name: id
  type: string
- description: Blueprint display name
  name: label
  type: string
- description: Data center fabric design type
  name: design
  type: string
- description: Current blueprint operational status
  name: status
  type: string
- description: Blueprint version number (incremented on deploy)
  name: version
  type: integer
- description: Number of intent-based analytics anomalies detected
  name: anomaly_count
  type: integer
- description: Number of build errors preventing deployment
  name: build_errors_count
  type: integer
- description: Number of build warnings
  name: build_warnings_count
  type: integer
- description: Fabric topology definition
  name: topology
  type: object
- description: Resource pool assignments
  name: resource_allocations
  type: object
- description: Virtual networks defined in the blueprint
  name: virtual_networks
  type: array
- description: Routing zones (VRFs) in the blueprint
  name: security_zones
  type: array
- description: Design template used to create this blueprint
  name: template_id
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: last_modified_at
  type: string
- description: ''
  name: last_deployed_at
  type: string
provider_name: Juniper Networks
provider_slug: juniper
schema_file: json-schema/juniper-blueprint.json
slug: juniper-blueprint
source_filename: juniper-blueprint.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/juniper/json-schema/juniper-blueprint.json\",\n  \"title\": \"Juniper Apstra Blueprint\",\n  \"description\": \"Schema representing a Juniper Apstra data center blueprint. A blueprint is the core abstraction in Apstra that defines the intended state of a data center fabric, including its topology, resource allocations, virtual networks, and policies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique blueprint identifier\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Blueprint display name\"\n    },\n    \"design\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"two_stage_l3clos\",\n        \"freeform\"\n      ],\n      \"description\": \"Data center fabric design type\"\n    },\n    \"status\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Current blueprint operational status\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Blueprint version number (incremented on deploy)\"\n    },\n    \"anomaly_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of intent-based analytics anomalies detected\"\n    },\n    \"build_errors_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of build errors preventing deployment\"\n    },\n    \"build_warnings_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of build warnings\"\n    },\n    \"topology\": {\n      \"type\": \"object\",\n      \"description\": \"Fabric topology definition\",\n      \"properties\": {\n        \"spine_count\": {\n          \"type\": \"integer\",\n          \"minimum\": 1\n        },\n        \"leaf_count\": {\n          \"type\": \"integer\",\n     \
  \     \"minimum\": 1\n        },\n        \"superspine_count\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"rack_count\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"resource_allocations\": {\n      \"type\": \"object\",\n      \"description\": \"Resource pool assignments\",\n      \"properties\": {\n        \"asn_pool_ids\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        },\n        \"ip_pool_ids\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        },\n        \"vni_pool_ids\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        }\n      }\n    },\n    \"virtual_networks\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Virtual networks defined in the blueprint\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"label\": {\n            \"type\": \"string\"\n          },\n          \"vn_type\": {\n            \"type\": \"string\",\n            \"enum\": [\"vxlan\", \"vlan\"]\n          },\n          \"security_zone_id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        }\n      }\n    },\n    \"security_zones\": {\n      \"type\": \"array\",\n      \"description\": \"Routing zones (VRFs) in the blueprint\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"label\": {\n            \"type\": \"string\"\n          },\n          \"vrf_name\": {\n            \"type\": \"string\"\
  \n          }\n        }\n      }\n    },\n    \"template_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Design template used to create this blueprint\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"last_modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"last_deployed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"id\", \"label\", \"design\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/json-schema/juniper-blueprint.json
tags:
- AI
- Automation
- Cloud
- Enterprise
- Networking
- SDN
- Security
title: Juniper Apstra Blueprint
---
