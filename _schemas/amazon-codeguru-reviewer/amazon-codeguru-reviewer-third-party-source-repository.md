---
description: Information about a third-party source repository connected to CodeGuru Reviewer.
layout: schema
name: ThirdPartySourceRepository
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: ConnectionArn
  type: object
- description: ''
  name: Owner
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-third-party-source-repository-schema.json
slug: amazon-codeguru-reviewer-third-party-source-repository
source_filename: amazon-codeguru-reviewer-third-party-source-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-third-party-source-repository-schema.json\",\n  \"title\": \"ThirdPartySourceRepository\",\n  \"description\": \"Information about a third-party source repository connected to CodeGuru Reviewer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the third party source repository.\"\n        }\n      ]\n    },\n    \"ConnectionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an Amazon Web Services CodeStar Connections connection. Its format is <code>arn:aws:codestar-connections:region-id:aws-account_id:connection/connection-id</code>.\
  \ For more information, see <a href=\\\"https://docs.aws.amazon.com/codestar-connections/latest/APIReference/API_Connection.html\\\">Connection</a> in the <i>Amazon Web Services CodeStar Connections API Reference</i>.\"\n        }\n      ]\n    },\n    \"Owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Owner\"\n        },\n        {\n          \"description\": \"The owner of the repository. For a GitHub, GitHub Enterprise, or Bitbucket repository, this is the username for the account that owns the repository. For an S3 repository, this can be the username or Amazon Web Services account ID \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"ConnectionArn\",\n    \"Owner\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-third-party-source-repository-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: ThirdPartySourceRepository
---
