---
description: GetOutpostInstanceTypesOutput schema from Amazon Outposts
layout: schema
name: GetOutpostInstanceTypesOutput
properties_list:
- description: ''
  name: InstanceTypes
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: OutpostId
  type: object
- description: ''
  name: OutpostArn
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-get-outpost-instance-types-output-schema.json
slug: openapi-get-outpost-instance-types-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-get-outpost-instance-types-output-schema.json\",\n  \"title\": \"GetOutpostInstanceTypesOutput\",\n  \"description\": \"GetOutpostInstanceTypesOutput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceTypes\": {\n      \"$ref\": \"#/components/schemas/InstanceTypeListDefinition\"\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/Token\"\n    },\n    \"OutpostId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutpostId\"\n        },\n        {\n          \"description\": \" The ID of the Outpost. \"\n        }\n      ]\n    },\n    \"OutpostArn\": {\n      \"$ref\": \"#/components/schemas/OutpostArn\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-get-outpost-instance-types-output-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: GetOutpostInstanceTypesOutput
---
