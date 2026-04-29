---
description: PutDefaultEncryptionConfigurationResponse schema
layout: schema
name: PutDefaultEncryptionConfigurationResponse
properties_list:
- description: ''
  name: encryptionType
  type: object
- description: ''
  name: kmsKeyArn
  type: object
- description: ''
  name: configurationStatus
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-put-default-encryption-configuration-response-schema.json
slug: iot-sitewise-put-default-encryption-configuration-response
source_filename: iot-sitewise-put-default-encryption-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-put-default-encryption-configuration-response-schema.json\",\n  \"title\": \"PutDefaultEncryptionConfigurationResponse\",\n  \"description\": \"PutDefaultEncryptionConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionType\"\n        },\n        {\n          \"description\": \"The type of encryption used for the encryption configuration.\"\n        }\n      ]\n    },\n    \"kmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The Key ARN of the KMS key used for KMS encryption if you use <code>KMS_BASED_ENCRYPTION</code>.\"\n        }\n      ]\n    },\n    \"\
  configurationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationStatus\"\n        },\n        {\n          \"description\": \"The status of the account configuration. This contains the <code>ConfigurationState</code>. If there is an error, it also contains the <code>ErrorDetails</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"encryptionType\",\n    \"configurationStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-put-default-encryption-configuration-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: PutDefaultEncryptionConfigurationResponse
---
