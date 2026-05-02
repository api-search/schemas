---
description: Schema for Neo4j AuraDB cloud database instances including configuration, status, and lifecycle management properties.
layout: schema
name: Neo4j Aura Instance
properties_list:
- description: Unique identifier for the AuraDB instance
  name: id
  type: string
- description: Display name of the instance
  name: name
  type: string
- description: Current lifecycle status of the instance
  name: status
  type: string
- description: Identifier of the tenant (project) this instance belongs to
  name: tenant_id
  type: string
- description: Cloud infrastructure provider hosting the instance
  name: cloud_provider
  type: string
- description: Cloud region where the instance is deployed
  name: region
  type: string
- description: Instance type determining capabilities and pricing tier
  name: type
  type: string
- description: Memory allocated to the instance
  name: memory
  type: string
- description: Storage allocated to the instance
  name: storage
  type: string
- description: Bolt connection URI for connecting to the instance
  name: connection_url
  type: string
- description: URL for the customer metrics integration endpoint
  name: metrics_integration_url
  type: string
- description: Neo4j database version running on the instance
  name: neo4j_version
  type: string
provider_name: Neo4j
provider_slug: neo4j
schema_file: json-schema/neo4j-aura-instance-schema.json
slug: neo4j-aura-instance
source_filename: neo4j-aura-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://neo4j.com/schemas/neo4j/aura-instance.json\",\n  \"title\": \"Neo4j Aura Instance\",\n  \"description\": \"Schema for Neo4j AuraDB cloud database instances including configuration, status, and lifecycle management properties.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\", \"tenant_id\", \"cloud_provider\", \"region\", \"type\", \"memory\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the AuraDB instance\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the instance\",\n      \"maxLength\": 30\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the instance\",\n      \"enum\": [\n        \"creating\",\n        \"running\",\n        \"pausing\",\n        \"paused\",\n        \"resuming\"\
  ,\n        \"updating\",\n        \"destroying\",\n        \"destroyed\",\n        \"loading\",\n        \"restoring\"\n      ]\n    },\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the tenant (project) this instance belongs to\"\n    },\n    \"cloud_provider\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud infrastructure provider hosting the instance\",\n      \"enum\": [\"gcp\", \"aws\", \"azure\"]\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud region where the instance is deployed\",\n      \"examples\": [\"us-east-1\", \"europe-west1\", \"eastus\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Instance type determining capabilities and pricing tier\",\n      \"enum\": [\n        \"enterprise-db\",\n        \"enterprise-ds\",\n        \"professional-db\",\n        \"free-db\"\n      ]\n    },\n    \"memory\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Memory allocated to the instance\",\n      \"pattern\": \"^\\\\d+GB$\",\n      \"examples\": [\"2GB\", \"8GB\", \"16GB\", \"32GB\"]\n    },\n    \"storage\": {\n      \"type\": \"string\",\n      \"description\": \"Storage allocated to the instance\",\n      \"pattern\": \"^\\\\d+GB$\",\n      \"examples\": [\"8GB\", \"16GB\", \"64GB\"]\n    },\n    \"connection_url\": {\n      \"type\": \"string\",\n      \"description\": \"Bolt connection URI for connecting to the instance\",\n      \"format\": \"uri\",\n      \"examples\": [\"neo4j+s://xxxxxxxx.databases.neo4j.io\"]\n    },\n    \"metrics_integration_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL for the customer metrics integration endpoint\",\n      \"format\": \"uri\"\n    },\n    \"neo4j_version\": {\n      \"type\": \"string\",\n      \"description\": \"Neo4j database version running on the instance\",\n      \"examples\": [\"5\"]\n    }\n  },\n  \"$defs\": {\n    \"Tenant\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"A tenant (project) that organizes and manages multiple AuraDB instances under a single administrative unit.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the tenant\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the tenant\"\n        },\n        \"instance_configurations\": {\n          \"type\": \"array\",\n          \"description\": \"Available instance configurations for this tenant\",\n          \"items\": {\n            \"$ref\": \"#/$defs/InstanceConfiguration\"\n          }\n        }\n      }\n    },\n    \"InstanceConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"An available instance configuration option within a tenant.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Instance type\"\n        },\n        \"regions\": {\n          \"type\": \"array\",\n          \"description\": \"Available cloud regions for this instance type\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Region identifier\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"Snapshot\": {\n      \"type\": \"object\",\n      \"description\": \"A point-in-time snapshot of an AuraDB instance for backup and restore purposes.\",\n      \"required\": [\"snapshot_id\", \"instance_id\", \"status\", \"timestamp\"],\n      \"properties\": {\n        \"snapshot_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the snapshot\"\n        },\n        \"instance_id\": {\n          \"type\": \"string\",\n          \"description\": \"Identifier of the instance this snapshot was taken\
  \ from\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current status of the snapshot\",\n          \"enum\": [\"Completed\", \"InProgress\", \"Failed\"]\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp of when the snapshot was created\"\n        },\n        \"exportable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the snapshot data can be exported\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/neo4j/refs/heads/main/json-schema/neo4j-aura-instance-schema.json
tags:
- Graph Database
- Cypher
- Cloud
- GraphQL
- Drivers
- APIs
title: Neo4j Aura Instance
---
