---
description: Details about a repository, including its Amazon Resource Name (ARN), description, and domain information. The <a href="https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_ListRepositories.html">ListRepositories</a> operation returns a list of <code>RepositorySummary</code> objects.
layout: schema
name: RepositorySummary
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: administratorAccount
  type: object
- description: ''
  name: domainName
  type: object
- description: ''
  name: domainOwner
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: createdTime
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-repository-summary-schema.json
slug: codeartifact-repository-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-repository-summary-schema.json\",\n  \"title\": \"RepositorySummary\",\n  \"description\": \" Details about a repository, including its Amazon Resource Name (ARN), description, and domain information. The <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_ListRepositories.html\\\">ListRepositories</a> operation returns a list of <code>RepositorySummary</code> objects. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \" The name of the repository. \"\n        }\n      ]\n    },\n    \"administratorAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n     \
  \   },\n        {\n          \"description\": \" The Amazon Web Services account ID that manages the repository. \"\n        }\n      ]\n    },\n    \"domainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \" The name of the domain that contains the repository. \"\n        }\n      ]\n    },\n    \"domainOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \" The 12-digit account number of the Amazon Web Services account that owns the domain. It does not include dashes or spaces. \"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \" The ARN of the repository. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Description\"\n        },\n        {\n          \"description\": \" The description of the repository. \"\n        }\n      ]\n    },\n    \"createdTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp that represents the date and time the repository was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-repository-summary-schema.json
tags:
- Amazon
- AWS
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
title: RepositorySummary
---
