---
description: Information about a domain. A domain is a container for repositories. When you create a domain, it is empty until you add one or more repositories.
layout: schema
name: DomainDescription
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: createdTime
  type: object
- description: ''
  name: encryptionKey
  type: object
- description: ''
  name: repositoryCount
  type: object
- description: ''
  name: assetSizeBytes
  type: object
- description: ''
  name: s3BucketArn
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-domain-description-schema.json
slug: codeartifact-domain-description
source_filename: codeartifact-domain-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-domain-description-schema.json\",\n  \"title\": \"DomainDescription\",\n  \"description\": \" Information about a domain. A domain is a container for repositories. When you create a domain, it is empty until you add one or more repositories. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \" The name of the domain. \"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \" The Amazon Web Services account ID that owns the domain. \"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the domain. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainStatus\"\n        },\n        {\n          \"description\": \" The current status of a domain. \"\n        }\n      ]\n    },\n    \"createdTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" A timestamp that represents the date and time the domain was created. \"\n        }\n      ]\n    },\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \" The ARN of an Key Management Service (KMS) key associated with a domain. \"\n        }\n      ]\n    },\n    \"repositoryCount\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of repositories in the domain. \"\n        }\n      ]\n    },\n    \"assetSizeBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \" The total size of all assets in the domain. \"\n        }\n      ]\n    },\n    \"s3BucketArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon S3 bucket that is used to store package assets in the domain.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-domain-description-schema.json
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
title: DomainDescription
---
