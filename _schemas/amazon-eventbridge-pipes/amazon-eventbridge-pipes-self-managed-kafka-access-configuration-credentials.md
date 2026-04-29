---
description: The Secrets Manager secret that stores your stream credentials.
layout: schema
name: SelfManagedKafkaAccessConfigurationCredentials
properties_list:
- description: ''
  name: BasicAuth
  type: object
- description: ''
  name: ClientCertificateTlsAuth
  type: object
- description: ''
  name: SaslScram256Auth
  type: object
- description: ''
  name: SaslScram512Auth
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-self-managed-kafka-access-configuration-credentials-schema.json
slug: amazon-eventbridge-pipes-self-managed-kafka-access-configuration-credentials
source_filename: amazon-eventbridge-pipes-self-managed-kafka-access-configuration-credentials-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-self-managed-kafka-access-configuration-credentials-schema.json\",\n  \"title\": \"SelfManagedKafkaAccessConfigurationCredentials\",\n  \"description\": \"The Secrets Manager secret that stores your stream credentials.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BasicAuth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretManagerArn\"\n        },\n        {\n          \"description\": \"The ARN of the Secrets Manager secret.\"\n        }\n      ]\n    },\n    \"ClientCertificateTlsAuth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretManagerArn\"\n        },\n        {\n          \"description\": \"The ARN of the Secrets Manager secret.\"\n        }\n      ]\n    },\n    \"SaslScram256Auth\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretManagerArn\"\n        },\n        {\n          \"description\": \"The ARN of the Secrets Manager secret.\"\n        }\n      ]\n    },\n    \"SaslScram512Auth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretManagerArn\"\n        },\n        {\n          \"description\": \"The ARN of the Secrets Manager secret.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-self-managed-kafka-access-configuration-credentials-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: SelfManagedKafkaAccessConfigurationCredentials
---
