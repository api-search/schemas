---
description: ListAssetsOutput schema from Amazon Outposts
layout: schema
name: ListAssetsOutput
properties_list:
- description: ''
  name: Assets
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-list-assets-output-schema.json
slug: openapi-list-assets-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-assets-output-schema.json\",\n  \"title\": \"ListAssetsOutput\",\n  \"description\": \"ListAssetsOutput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Assets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetListDefinition\"\n        },\n        {\n          \"description\": \"Information about the hardware assets.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/Token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-assets-output-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: ListAssetsOutput
---
