---
description: CancelChangeSetResponse schema from Amazon Marketplace API
layout: schema
name: CancelChangeSetResponse
properties_list:
- description: ''
  name: ChangeSetId
  type: object
- description: ''
  name: ChangeSetArn
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-cancel-change-set-response-schema.json
slug: amazon-marketplace-cancel-change-set-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-cancel-change-set-response-schema.json\",\n  \"title\": \"CancelChangeSetResponse\",\n  \"description\": \"CancelChangeSetResponse schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier for the change set referenced in this request.\"\n        }\n      ]\n    },\n    \"ChangeSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN associated with the change set referenced in this request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-cancel-change-set-response-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: CancelChangeSetResponse
---
