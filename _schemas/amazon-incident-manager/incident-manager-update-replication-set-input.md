---
description: UpdateReplicationSetInput schema
layout: schema
name: UpdateReplicationSetInput
properties_list:
- description: ''
  name: actions
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-update-replication-set-input-schema.json
slug: incident-manager-update-replication-set-input
source_filename: incident-manager-update-replication-set-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-replication-set-input-schema.json\",\n  \"title\": \"UpdateReplicationSetInput\",\n  \"description\": \"UpdateReplicationSetInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateReplicationSetInputActionsList\"\n        },\n        {\n          \"description\": \"An action to add or delete a Region.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the replication set you're updating.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\
  \n        },\n        {\n          \"description\": \"A token that ensures that the operation is called only once with the specified details.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"actions\",\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-replication-set-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: UpdateReplicationSetInput
---
