---
description: The details of a repository stored in CodeArtifact. A CodeArtifact repository contains a set of package versions, each of which maps to a set of assets. Repositories are polyglot—a single repository can contain packages of any supported type. Each repository exposes endpoints for fetching and publishing packages using tools like the <code>npm</code> CLI, the Maven CLI (<code>mvn</code>), and <code>pip</code>. You can create up to 100 repositories per Amazon Web Services account.
layout: schema
name: RepositoryDescription
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
  name: upstreams
  type: object
- description: ''
  name: externalConnections
  type: object
- description: ''
  name: createdTime
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-repository-description-schema.json
slug: codeartifact-repository-description
source_filename: codeartifact-repository-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-repository-description-schema.json\",\n  \"title\": \"RepositoryDescription\",\n  \"description\": \" The details of a repository stored in CodeArtifact. A CodeArtifact repository contains a set of package versions, each of which maps to a set of assets. Repositories are polyglot\\u2014a single repository can contain packages of any supported type. Each repository exposes endpoints for fetching and publishing packages using tools like the <code>npm</code> CLI, the Maven CLI (<code>mvn</code>), and <code>pip</code>. You can create up to 100 repositories per Amazon Web Services account. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\"\
  : \" The name of the repository. \"\n        }\n      ]\n    },\n    \"administratorAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \" The 12-digit account number of the Amazon Web Services account that manages the repository. \"\n        }\n      ]\n    },\n    \"domainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \" The name of the domain that contains the repository. \"\n        }\n      ]\n    },\n    \"domainOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \" The 12-digit account number of the Amazon Web Services account that owns the domain that contains the repository. It does not include dashes or spaces. \"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the repository. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \" A text description of the repository. \"\n        }\n      ]\n    },\n    \"upstreams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpstreamRepositoryInfoList\"\n        },\n        {\n          \"description\": \" A list of upstream repositories to associate with the repository. The order of the upstream repositories in the list determines their priority order when CodeArtifact looks for a requested package version. For more information, see <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/ug/repos-upstream.html\\\">Working with upstream repositories</a>. \"\n        }\n      ]\n    },\n\
  \    \"externalConnections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryExternalConnectionInfoList\"\n        },\n        {\n          \"description\": \" An array of external connections associated with the repository. \"\n        }\n      ]\n    },\n    \"createdTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp that represents the date and time the repository was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-repository-description-schema.json
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
title: RepositoryDescription
---
