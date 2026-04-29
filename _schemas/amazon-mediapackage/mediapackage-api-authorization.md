---
description: CDN Authorization credentials
layout: schema
name: Authorization
properties_list:
- description: ''
  name: CdnIdentifierSecret
  type: object
- description: ''
  name: SecretsRoleArn
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-authorization-schema.json
slug: mediapackage-api-authorization
source_filename: mediapackage-api-authorization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-authorization-schema.json\",\n  \"title\": \"Authorization\",\n  \"description\": \"CDN Authorization credentials\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CdnIdentifierSecret\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cdnIdentifierSecret\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) for the secret in Secrets Manager that your Content Distribution Network (CDN) uses for authorization to access your endpoint.\\n\"\n        }\n      ]\n    },\n    \"SecretsRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"\
  secretsRoleArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) for the IAM role that allows MediaPackage to communicate with AWS Secrets Manager.\\n\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SecretsRoleArn\",\n    \"CdnIdentifierSecret\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-authorization-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Authorization
---
