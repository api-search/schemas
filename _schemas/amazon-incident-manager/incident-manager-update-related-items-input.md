---
description: UpdateRelatedItemsInput schema
layout: schema
name: UpdateRelatedItemsInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: incidentRecordArn
  type: object
- description: ''
  name: relatedItemsUpdate
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-update-related-items-input-schema.json
slug: incident-manager-update-related-items-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-related-items-input-schema.json\",\n  \"title\": \"UpdateRelatedItemsInput\",\n  \"description\": \"UpdateRelatedItemsInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A token that ensures that a client calls the operation only once with the specified details.\"\n        }\n      ]\n    },\n    \"incidentRecordArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the incident record that contains the related items that you update.\"\n        }\n      ]\n    },\n    \"relatedItemsUpdate\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelatedItemsUpdate\"\n        },\n        {\n          \"description\": \"Details about the item that you are add to, or delete from, an incident.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"incidentRecordArn\",\n    \"relatedItemsUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-related-items-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: UpdateRelatedItemsInput
---
