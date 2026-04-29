---
description: Specifies the configuration settings for retrieving occurrences of sensitive data reported by findings, and the status of the configuration for an Amazon Macie account. When you enable the configuration for the first time, your request must specify an Key Management Service (KMS) key. Otherwise, an error occurs. Macie uses the specified key to encrypt the sensitive data that you retrieve.
layout: schema
name: RevealConfiguration
properties_list:
- description: ''
  name: kmsKeyId
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-reveal-configuration-schema.json
slug: amazon-macie-reveal-configuration
source_filename: amazon-macie-reveal-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-reveal-configuration-schema.json\",\n  \"title\": \"RevealConfiguration\",\n  \"description\": \"Specifies the configuration settings for retrieving occurrences of sensitive data reported by findings, and the status of the configuration for an Amazon Macie account. When you enable the configuration for the first time, your request must specify an Key Management Service (KMS) key. Otherwise, an error occurs. Macie uses the specified key to encrypt the sensitive data that you retrieve.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max2048\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN), ID, or alias of the KMS key to use to encrypt sensitive data\
  \ that's retrieved. The key must be an existing, customer managed, symmetric encryption key that's in the same Amazon Web Services Region as the Amazon Macie account.</p> <p>If this value specifies an alias, it must include the following prefix: alias/. If this value specifies a key that's owned by another Amazon Web Services account, it must specify the ARN of the key or the ARN of the key's alias.</p>\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevealStatus\"\n        },\n        {\n          \"description\": \"The status of the configuration for the Amazon Macie account. In a request, valid values are: ENABLED, enable the configuration for the account; and, DISABLED, disable the configuration for the account. In a response, possible values are: ENABLED, the configuration is currently enabled for the account; and, DISABLED, the configuration is currently disabled for the account.\"\n        }\n      ]\n \
  \   }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-reveal-configuration-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: RevealConfiguration
---
