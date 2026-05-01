---
description: ListEnvironmentsOutput schema from Amazon Proton API
layout: schema
name: ListEnvironmentsOutput
properties_list:
- description: ''
  name: environments
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-environments-output-schema.json
slug: amazon-proton-list-environments-output
source_filename: amazon-proton-list-environments-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environments-output-schema.json\",\n  \"title\": \"ListEnvironmentsOutput\",\n  \"description\": \"ListEnvironmentsOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentSummaryList\"\n        },\n        {\n          \"description\": \"An array of environment detail data summaries.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next environment in the array of environments, after the current requested list of environments.\"\n        }\n      ]\n    }\n  },\n \
  \ \"required\": [\n    \"environments\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environments-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListEnvironmentsOutput
---
