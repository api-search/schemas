---
description: CreateReplicationSetInput schema
layout: schema
name: CreateReplicationSetInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: regions
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-create-replication-set-input-schema.json
slug: incident-manager-create-replication-set-input
source_filename: incident-manager-create-replication-set-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-create-replication-set-input-schema.json\",\n  \"title\": \"CreateReplicationSetInput\",\n  \"description\": \"CreateReplicationSetInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A token that ensures that the operation is called only once with the specified details.\"\n        }\n      ]\n    },\n    \"regions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionMapInput\"\n        },\n        {\n          \"description\": \"The Regions that Incident Manager replicates your data to. You can have up to three Regions in your replication set.\"\n        }\n      ]\n    },\n\
  \    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of tags to add to the replication set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"regions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-create-replication-set-input-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: CreateReplicationSetInput
---
