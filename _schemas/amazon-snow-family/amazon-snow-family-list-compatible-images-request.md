---
description: ListCompatibleImagesRequest schema from Amazon Snow Family API
layout: schema
name: ListCompatibleImagesRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-list-compatible-images-request-schema.json
slug: amazon-snow-family-list-compatible-images-request
source_filename: amazon-snow-family-list-compatible-images-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-compatible-images-request-schema.json\",\n  \"title\": \"ListCompatibleImagesRequest\",\n  \"description\": \"ListCompatibleImagesRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListLimit\"\n        },\n        {\n          \"description\": \"The maximum number of results for the list of compatible images. Currently, a Snowball Edge device can store 10 AMIs.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"HTTP requests are stateless. To identify what object comes \\\"next\\\" in the list of compatible\
  \ images, you can specify a value for <code>NextToken</code> as the starting point for your list of returned images.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-compatible-images-request-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ListCompatibleImagesRequest
---
