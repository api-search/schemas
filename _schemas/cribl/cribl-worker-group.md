---
description: A Cribl worker group or edge fleet that organizes nodes and deploys shared configurations for processing observability data at scale.
layout: schema
name: Cribl Worker Group
properties_list:
- description: Unique identifier for the worker group or fleet
  name: id
  type: string
- description: Display name for the group
  name: name
  type: string
- description: A human-readable description of the group purpose
  name: description
  type: string
- description: Whether this group is an edge fleet rather than a stream worker group
  name: isFleet
  type: boolean
- description: Number of connected worker or edge nodes in this group
  name: workerCount
  type: integer
- description: The currently deployed configuration version identifier
  name: configVersion
  type: string
- description: Key-value tags for organizing and categorizing groups
  name: tags
  type: object
- description: Whether the group has been provisioned and is ready to accept nodes
  name: provisioned
  type: boolean
- description: Cloud-specific configuration for Cribl Cloud deployments
  name: cloud
  type: object
provider_name: Cribl
provider_slug: cribl
schema_file: json-schema/cribl-worker-group-schema.json
slug: cribl-worker-group
source_filename: cribl-worker-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.cribl.io/schemas/cribl/worker-group.json\",\n  \"title\": \"Cribl Worker Group\",\n  \"description\": \"A Cribl worker group or edge fleet that organizes nodes and deploys shared configurations for processing observability data at scale.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the worker group or fleet\",\n      \"pattern\": \"^[a-zA-Z0-9_-]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the group\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the group purpose\"\n    },\n    \"isFleet\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this group is an edge fleet rather than a stream worker group\",\n      \"\
  default\": false\n    },\n    \"workerCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of connected worker or edge nodes in this group\",\n      \"minimum\": 0\n    },\n    \"configVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The currently deployed configuration version identifier\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value tags for organizing and categorizing groups\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"provisioned\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the group has been provisioned and is ready to accept nodes\"\n    },\n    \"cloud\": {\n      \"type\": \"object\",\n      \"description\": \"Cloud-specific configuration for Cribl Cloud deployments\",\n      \"properties\": {\n        \"provider\": {\n          \"type\": \"string\",\n          \"description\": \"The cloud provider\",\n          \"enum\": [\"\
  aws\", \"azure\", \"gcp\"]\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"The cloud region for the worker group\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/json-schema/cribl-worker-group-schema.json
tags:
- Configuration
- Data Lake
- Data Pipelines
- Data Routing
- Edge Computing
- Infrastructure as Code
- Observability
- Search
- Security Data
- Stream Processing
- Telemetry
title: Cribl Worker Group
---
