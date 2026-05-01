---
description: ListComponentsOutput schema from Amazon Proton API
layout: schema
name: ListComponentsOutput
properties_list:
- description: ''
  name: components
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-components-output-schema.json
slug: amazon-proton-list-components-output
source_filename: amazon-proton-list-components-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-components-output-schema.json\",\n  \"title\": \"ListComponentsOutput\",\n  \"description\": \"ListComponentsOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentSummaryList\"\n        },\n        {\n          \"description\": \"An array of components with summary data.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next component in the array of components, after the current requested list of components.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n   \
  \ \"components\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-components-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListComponentsOutput
---
