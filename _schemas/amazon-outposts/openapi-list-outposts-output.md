---
description: ListOutpostsOutput schema from Amazon Outposts
layout: schema
name: ListOutpostsOutput
properties_list:
- description: ''
  name: Outposts
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-list-outposts-output-schema.json
slug: openapi-list-outposts-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-outposts-output-schema.json\",\n  \"title\": \"ListOutpostsOutput\",\n  \"description\": \"ListOutpostsOutput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Outposts\": {\n      \"$ref\": \"#/components/schemas/outpostListDefinition\"\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/Token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-outposts-output-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: ListOutpostsOutput
---
