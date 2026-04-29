---
description: Information about an associated Amazon Web Services CodeCommit repository or an associated repository that is managed by Amazon Web Services CodeStar Connections (for example, Bitbucket). This <code>Repository</code> object is not used if your source code is in an associated GitHub repository.
layout: schema
name: Repository
properties_list:
- description: ''
  name: CodeCommit
  type: object
- description: ''
  name: Bitbucket
  type: object
- description: ''
  name: GitHubEnterpriseServer
  type: object
- description: ''
  name: S3Bucket
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-repository-schema.json
slug: amazon-codeguru-reviewer-repository
source_filename: amazon-codeguru-reviewer-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-repository-schema.json\",\n  \"title\": \"Repository\",\n  \"description\": \"Information about an associated Amazon Web Services CodeCommit repository or an associated repository that is managed by Amazon Web Services CodeStar Connections (for example, Bitbucket). This <code>Repository</code> object is not used if your source code is in an associated GitHub repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeCommit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeCommitRepository\"\n        },\n        {\n          \"description\": \"Information about an Amazon Web Services CodeCommit repository.\"\n        }\n      ]\n    },\n    \"Bitbucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThirdPartySourceRepository\"\
  \n        },\n        {\n          \"description\": \" Information about a Bitbucket repository. \"\n        }\n      ]\n    },\n    \"GitHubEnterpriseServer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThirdPartySourceRepository\"\n        },\n        {\n          \"description\": \"Information about a GitHub Enterprise Server repository.\"\n        }\n      ]\n    },\n    \"S3Bucket\": {\n      \"$ref\": \"#/components/schemas/S3Repository\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-repository-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: Repository
---
