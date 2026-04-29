---
description: ListEnvironmentTemplatesInput schema from Amazon Proton API
layout: schema
name: ListEnvironmentTemplatesInput
properties_list:
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-environment-templates-input-schema.json
slug: amazon-proton-list-environment-templates-input
source_filename: amazon-proton-list-environment-templates-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-templates-input-schema.json\",\n  \"title\": \"ListEnvironmentTemplatesInput\",\n  \"description\": \"ListEnvironmentTemplatesInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxPageResults\"\n        },\n        {\n          \"description\": \"The maximum number of environment templates to list.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next environment template in the array of environment templates, after the list of environment templates that was previously\
  \ requested.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-templates-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListEnvironmentTemplatesInput
---
