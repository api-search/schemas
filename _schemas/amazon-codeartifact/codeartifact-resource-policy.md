---
description: An CodeArtifact resource policy that contains a resource ARN, document details, and a revision.
layout: schema
name: ResourcePolicy
properties_list:
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: revision
  type: object
- description: ''
  name: document
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-resource-policy-schema.json
slug: codeartifact-resource-policy
source_filename: codeartifact-resource-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-resource-policy-schema.json\",\n  \"title\": \"ResourcePolicy\",\n  \"description\": \" An CodeArtifact resource policy that contains a resource ARN, document details, and a revision. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \" The ARN of the resource associated with the resource policy \"\n        }\n      ]\n    },\n    \"revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRevision\"\n        },\n        {\n          \"description\": \" The current revision of the resource policy. \"\n        }\n      ]\n    },\n    \"document\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \" The resource policy formatted in JSON. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-resource-policy-schema.json
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
title: ResourcePolicy
---
