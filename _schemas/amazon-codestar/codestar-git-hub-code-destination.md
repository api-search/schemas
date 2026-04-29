---
description: Information about the GitHub repository to be created in AWS CodeStar. This is where the source code files provided with the project request will be uploaded after project creation.
layout: schema
name: GitHubCodeDestination
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: privateRepository
  type: object
- description: ''
  name: issuesEnabled
  type: object
- description: ''
  name: token
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-git-hub-code-destination-schema.json
slug: codestar-git-hub-code-destination
source_filename: codestar-git-hub-code-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-git-hub-code-destination-schema.json\",\n  \"title\": \"GitHubCodeDestination\",\n  \"description\": \"Information about the GitHub repository to be created in AWS CodeStar. This is where the source code files provided with the project request will be uploaded after project creation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \"Name of the GitHub repository to be created in AWS CodeStar.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryDescription\"\n        },\n        {\n          \"description\": \"Description for the GitHub repository to\
  \ be created in AWS CodeStar. This description displays in GitHub after the repository is created.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryType\"\n        },\n        {\n          \"description\": \"The type of GitHub repository to be created in AWS CodeStar. Valid values are User or Organization.\"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryOwner\"\n        },\n        {\n          \"description\": \"The GitHub username for the owner of the GitHub repository to be created in AWS CodeStar. If this repository should be owned by a GitHub organization, provide its name.\"\n        }\n      ]\n    },\n    \"privateRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryIsPrivate\"\n        },\n        {\n          \"description\": \"Whether the GitHub repository is to\
  \ be a private repository.\"\n        }\n      ]\n    },\n    \"issuesEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryEnableIssues\"\n        },\n        {\n          \"description\": \"Whether to enable issues for the GitHub repository.\"\n        }\n      ]\n    },\n    \"token\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitHubPersonalToken\"\n        },\n        {\n          \"description\": \"The GitHub user's personal access token for the GitHub repository.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\",\n    \"owner\",\n    \"privateRepository\",\n    \"issuesEnabled\",\n    \"token\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-git-hub-code-destination-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: GitHubCodeDestination
---
