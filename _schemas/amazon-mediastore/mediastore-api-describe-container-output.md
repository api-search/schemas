---
description: DescribeContainerOutput schema from Amazon MediaStore API
layout: schema
name: DescribeContainerOutput
properties_list:
- description: ''
  name: Container
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-describe-container-output-schema.json
slug: mediastore-api-describe-container-output
source_filename: mediastore-api-describe-container-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-describe-container-output-schema.json\",\n  \"title\": \"DescribeContainerOutput\",\n  \"description\": \"DescribeContainerOutput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Container\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Container\"\n        },\n        {\n          \"description\": \"The name of the queried container.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-describe-container-output-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DescribeContainerOutput
---
