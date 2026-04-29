---
description: ListEnvironmentAccountConnectionsInput schema from Amazon Proton API
layout: schema
name: ListEnvironmentAccountConnectionsInput
properties_list:
- description: ''
  name: environmentName
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: requestedBy
  type: object
- description: ''
  name: statuses
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-environment-account-connections-input-schema.json
slug: amazon-proton-list-environment-account-connections-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-account-connections-input-schema.json\",\n  \"title\": \"ListEnvironmentAccountConnectionsInput\",\n  \"description\": \"ListEnvironmentAccountConnectionsInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The environment name that's associated with each listed environment account connection.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxPageResults\"\n        },\n        {\n          \"description\": \"The maximum number of environment account connections to list.\"\n        }\n      ]\n \
  \   },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next environment account connection in the array of environment account connections, after the list of environment account connections that was previously requested.\"\n        }\n      ]\n    },\n    \"requestedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionRequesterAccountType\"\n        },\n        {\n          \"description\": \"The type of account making the <code>ListEnvironmentAccountConnections</code> request.\"\n        }\n      ]\n    },\n    \"statuses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionStatusList\"\n        },\n        {\n          \"description\": \"The status details for each listed environment account connection.\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"requestedBy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-account-connections-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListEnvironmentAccountConnectionsInput
---
