---
description: Provides information about an action that occurred for a resource and produced a policy finding.
layout: schema
name: FindingAction
properties_list:
- description: ''
  name: actionType
  type: object
- description: ''
  name: apiCallDetails
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-finding-action-schema.json
slug: amazon-macie-finding-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-action-schema.json\",\n  \"title\": \"FindingAction\",\n  \"description\": \"Provides information about an action that occurred for a resource and produced a policy finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingActionType\"\n        },\n        {\n          \"description\": \"The type of action that occurred for the affected resource. This value is typically AWS_API_CALL, which indicates that an entity invoked an API operation for the resource.\"\n        }\n      ]\n    },\n    \"apiCallDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApiCallDetails\"\n        },\n        {\n          \"description\": \"The invocation details of the\
  \ API operation that an entity invoked for the affected resource, if the value for the actionType property is AWS_API_CALL.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-action-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: FindingAction
---
