---
description: Represents the input of a <code>DeleteGitHubAccount</code> operation.
layout: schema
name: DeleteGitHubAccountTokenInput
properties_list:
- description: ''
  name: tokenName
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-delete-git-hub-account-token-input-schema.json
slug: amazon-codedeploy-delete-git-hub-account-token-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-delete-git-hub-account-token-input-schema.json\",\n  \"title\": \"DeleteGitHubAccountTokenInput\",\n  \"description\": \"Represents the input of a <code>DeleteGitHubAccount</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokenName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitHubAccountTokenName\"\n        },\n        {\n          \"description\": \"The name of the GitHub account connection to delete.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-delete-git-hub-account-token-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeleteGitHubAccountTokenInput
---
