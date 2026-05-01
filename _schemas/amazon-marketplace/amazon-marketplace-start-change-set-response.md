---
description: StartChangeSetResponse schema from Amazon Marketplace API
layout: schema
name: StartChangeSetResponse
properties_list:
- description: ''
  name: ChangeSetId
  type: object
- description: ''
  name: ChangeSetArn
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-start-change-set-response-schema.json
slug: amazon-marketplace-start-change-set-response
source_filename: amazon-marketplace-start-change-set-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-start-change-set-response-schema.json\",\n  \"title\": \"StartChangeSetResponse\",\n  \"description\": \"StartChangeSetResponse schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"Unique identifier generated for the request.\"\n        }\n      ]\n    },\n    \"ChangeSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN associated to the unique identifier generated for the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-start-change-set-response-schema.json
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
title: StartChangeSetResponse
---
