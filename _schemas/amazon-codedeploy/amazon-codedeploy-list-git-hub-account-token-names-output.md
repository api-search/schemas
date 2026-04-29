---
description: Represents the output of a <code>ListGitHubAccountTokenNames</code> operation.
layout: schema
name: ListGitHubAccountTokenNamesOutput
properties_list:
- description: ''
  name: tokenNameList
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-git-hub-account-token-names-output-schema.json
slug: amazon-codedeploy-list-git-hub-account-token-names-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-git-hub-account-token-names-output-schema.json\",\n  \"title\": \"ListGitHubAccountTokenNamesOutput\",\n  \"description\": \"Represents the output of a <code>ListGitHubAccountTokenNames</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokenNameList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitHubAccountTokenNameList\"\n        },\n        {\n          \"description\": \"A list of names of connections to GitHub accounts.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If a large amount of information is returned, an identifier is also returned. It can be used in a subsequent\
  \ <code>ListGitHubAccountTokenNames</code> call to return the next set of names in the list. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-git-hub-account-token-names-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListGitHubAccountTokenNamesOutput
---
