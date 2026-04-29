---
description: ListEnvironmentTemplatesOutput schema from Amazon Proton API
layout: schema
name: ListEnvironmentTemplatesOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: templates
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-environment-templates-output-schema.json
slug: amazon-proton-list-environment-templates-output
source_filename: amazon-proton-list-environment-templates-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-templates-output-schema.json\",\n  \"title\": \"ListEnvironmentTemplatesOutput\",\n  \"description\": \"ListEnvironmentTemplatesOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next environment template in the array of environment templates, after the current requested list of environment templates.\"\n        }\n      ]\n    },\n    \"templates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentTemplateSummaryList\"\n        },\n        {\n          \"description\": \"An array of environment templates\
  \ with detail data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"templates\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-templates-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListEnvironmentTemplatesOutput
---
