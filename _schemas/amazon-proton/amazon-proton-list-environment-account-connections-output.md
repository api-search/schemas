---
description: ListEnvironmentAccountConnectionsOutput schema from Amazon Proton API
layout: schema
name: ListEnvironmentAccountConnectionsOutput
properties_list:
- description: ''
  name: environmentAccountConnections
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-environment-account-connections-output-schema.json
slug: amazon-proton-list-environment-account-connections-output
source_filename: amazon-proton-list-environment-account-connections-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-account-connections-output-schema.json\",\n  \"title\": \"ListEnvironmentAccountConnectionsOutput\",\n  \"description\": \"ListEnvironmentAccountConnectionsOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentAccountConnections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionSummaryList\"\n        },\n        {\n          \"description\": \"An array of environment account connections with details that's returned by Proton. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next environment\
  \ account connection in the array of environment account connections, after the current requested list of environment account connections.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"environmentAccountConnections\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-account-connections-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListEnvironmentAccountConnectionsOutput
---
