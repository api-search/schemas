---
description: Information about the location of application artifacts stored in GitHub.
layout: schema
name: GitHubLocation
properties_list:
- description: ''
  name: repository
  type: object
- description: ''
  name: commitId
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-git-hub-location-schema.json
slug: amazon-codedeploy-git-hub-location
source_filename: amazon-codedeploy-git-hub-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-git-hub-location-schema.json\",\n  \"title\": \"GitHubLocation\",\n  \"description\": \"Information about the location of application artifacts stored in GitHub.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Repository\"\n        },\n        {\n          \"description\": \"<p>The GitHub account and repository pair that stores a reference to the commit that represents the bundled artifacts for the application revision. </p> <p>Specified as account/repository.</p>\"\n        }\n      ]\n    },\n    \"commitId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CommitId\"\n        },\n        {\n          \"description\": \"The SHA1 commit ID of the GitHub commit\
  \ that represents the bundled artifacts for the application revision.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-git-hub-location-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GitHubLocation
---
