---
description: ListCompatibleImagesResult schema from Amazon Snow Family API
layout: schema
name: ListCompatibleImagesResult
properties_list:
- description: ''
  name: CompatibleImages
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-list-compatible-images-result-schema.json
slug: amazon-snow-family-list-compatible-images-result
source_filename: amazon-snow-family-list-compatible-images-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-compatible-images-result-schema.json\",\n  \"title\": \"ListCompatibleImagesResult\",\n  \"description\": \"ListCompatibleImagesResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CompatibleImages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompatibleImageList\"\n        },\n        {\n          \"description\": \"A JSON-formatted object that describes a compatible AMI, including the ID and name for a Snow device AMI.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Because HTTP requests are stateless, this is the starting point for your next list of returned\
  \ images.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-compatible-images-result-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ListCompatibleImagesResult
---
