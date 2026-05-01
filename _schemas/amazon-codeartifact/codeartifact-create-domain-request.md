---
description: CreateDomainRequest schema from Amazon CodeArtifact API
layout: schema
name: CreateDomainRequest
properties_list:
- description: ''
  name: encryptionKey
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-create-domain-request-schema.json
slug: codeartifact-create-domain-request
source_filename: codeartifact-create-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-create-domain-request-schema.json\",\n  \"title\": \"CreateDomainRequest\",\n  \"description\": \"CreateDomainRequest schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p> The encryption key for the domain. This is used to encrypt content stored in a domain. An encryption key can be a key ID, a key Amazon Resource Name (ARN), a key alias, or a key alias ARN. To specify an <code>encryptionKey</code>, your IAM role must have <code>kms:DescribeKey</code> and <code>kms:CreateGrant</code> permissions on the encryption key that is used. For more information, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/APIReference/API_DescribeKey.html#API_DescribeKey_RequestSyntax\\\
  \">DescribeKey</a> in the <i>Key Management Service API Reference</i> and <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/kms-api-permissions-reference.html\\\">Key Management Service API Permissions Reference</a> in the <i>Key Management Service Developer Guide</i>. </p> <important> <p> CodeArtifact supports only symmetric CMKs. Do not associate an asymmetric CMK with your domain. For more information, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/symmetric-asymmetric.html\\\">Using symmetric and asymmetric keys</a> in the <i>Key Management Service Developer Guide</i>. </p> </important>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"One or more tag key-value pairs for the domain.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-create-domain-request-schema.json
tags:
- Amazon
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
title: CreateDomainRequest
---
