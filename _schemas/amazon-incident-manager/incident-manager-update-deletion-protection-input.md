---
description: UpdateDeletionProtectionInput schema
layout: schema
name: UpdateDeletionProtectionInput
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: deletionProtected
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-update-deletion-protection-input-schema.json
slug: incident-manager-update-deletion-protection-input
source_filename: incident-manager-update-deletion-protection-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-deletion-protection-input-schema.json\",\n  \"title\": \"UpdateDeletionProtectionInput\",\n  \"description\": \"UpdateDeletionProtectionInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the replication set to update.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A token that ensures that the operation is called only once with the specified details.\"\n        }\n      ]\n    },\n    \"deletionProtected\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies if deletion protection is turned on or off in your account. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"deletionProtected\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-deletion-protection-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: UpdateDeletionProtectionInput
---
