---
description: Describes a custom encryption key that App Runner uses to encrypt copies of the source repository and service logs.
layout: schema
name: EncryptionConfiguration
properties_list:
- description: ''
  name: KmsKey
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-encryptionconfiguration-schema.json
slug: amazon-app-runner-encryptionconfiguration
source_filename: amazon-app-runner-encryptionconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"EncryptionConfiguration\",\n  \"description\": \"Describes a custom encryption key that App Runner uses to encrypt copies of the source repository and service logs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KmsKey\": {}\n  },\n  \"required\": [\n    \"KmsKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-encryptionconfiguration-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: EncryptionConfiguration
---
