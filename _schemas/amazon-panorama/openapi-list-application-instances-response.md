---
description: ListApplicationInstancesResponse schema from Amazon Panorama
layout: schema
name: ListApplicationInstancesResponse
properties_list:
- description: ''
  name: ApplicationInstances
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-list-application-instances-response-schema.json
slug: openapi-list-application-instances-response
source_filename: openapi-list-application-instances-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-list-application-instances-response-schema.json\",\n  \"title\": \"ListApplicationInstancesResponse\",\n  \"description\": \"ListApplicationInstancesResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstances\"\n        },\n        {\n          \"description\": \"A list of application instances.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-list-application-instances-response-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: ListApplicationInstancesResponse
---
