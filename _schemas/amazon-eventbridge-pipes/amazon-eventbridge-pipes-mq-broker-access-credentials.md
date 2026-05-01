---
description: The Secrets Manager secret that stores your broker credentials.
layout: schema
name: MQBrokerAccessCredentials
properties_list:
- description: ''
  name: BasicAuth
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-mq-broker-access-credentials-schema.json
slug: amazon-eventbridge-pipes-mq-broker-access-credentials
source_filename: amazon-eventbridge-pipes-mq-broker-access-credentials-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-mq-broker-access-credentials-schema.json\",\n  \"title\": \"MQBrokerAccessCredentials\",\n  \"description\": \"The Secrets Manager secret that stores your broker credentials.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BasicAuth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretManagerArn\"\n        },\n        {\n          \"description\": \"The ARN of the Secrets Manager secret.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-mq-broker-access-credentials-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: MQBrokerAccessCredentials
---
