---
description: ListPackagesResponse schema from Amazon Panorama
layout: schema
name: ListPackagesResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Packages
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-list-packages-response-schema.json
slug: openapi-list-packages-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-list-packages-response-schema.json\",\n  \"title\": \"ListPackagesResponse\",\n  \"description\": \"ListPackagesResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    },\n    \"Packages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageList\"\n        },\n        {\n          \"description\": \"A list of packages.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-list-packages-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: ListPackagesResponse
---
