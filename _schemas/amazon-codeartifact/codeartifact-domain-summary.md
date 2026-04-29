---
description: Information about a domain, including its name, Amazon Resource Name (ARN), and status. The <a href="https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_ListDomains.html">ListDomains</a> operation returns a list of <code>DomainSummary</code> objects.
layout: schema
name: DomainSummary
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
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-domain-summary-schema.json
slug: codeartifact-domain-summary
source_filename: codeartifact-domain-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-domain-summary-schema.json\",\n  \"title\": \"DomainSummary\",\n  \"description\": \" Information about a domain, including its name, Amazon Resource Name (ARN), and status. The <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_ListDomains.html\\\">ListDomains</a> operation returns a list of <code>DomainSummary</code> objects. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \" The name of the domain. \"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \" The 12-digit account\
  \ number of the Amazon Web Services account that owns the domain. It does not include dashes or spaces. \"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \" The ARN of the domain. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainStatus\"\n        },\n        {\n          \"description\": \" A string that contains the status of the domain. \"\n        }\n      ]\n    },\n    \"createdTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" A timestamp that contains the date and time the domain was created. \"\n        }\n      ]\n    },\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\"\
  : \" The key used to encrypt the domain. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-domain-summary-schema.json
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
title: DomainSummary
---
