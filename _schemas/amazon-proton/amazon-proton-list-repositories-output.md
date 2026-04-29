---
description: ListRepositoriesOutput schema from Amazon Proton API
layout: schema
name: ListRepositoriesOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: repositories
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-repositories-output-schema.json
slug: amazon-proton-list-repositories-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-repositories-output-schema.json\",\n  \"title\": \"ListRepositoriesOutput\",\n  \"description\": \"ListRepositoriesOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next repository in the array of repositories, after the current requested list of repositories. \"\n        }\n      ]\n    },\n    \"repositories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositorySummaryList\"\n        },\n        {\n          \"description\": \"An array of repository links.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"repositories\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-repositories-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListRepositoriesOutput
---
