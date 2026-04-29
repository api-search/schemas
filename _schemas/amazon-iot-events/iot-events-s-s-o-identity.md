---
description: Contains information about your identity source in AWS Single Sign-On. For more information, see the <a href="https://docs.aws.amazon.com/singlesignon/latest/userguide/what-is.html">AWS Single Sign-On User Guide</a>.
layout: schema
name: SSOIdentity
properties_list:
- description: ''
  name: identityStoreId
  type: object
- description: ''
  name: userId
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-s-s-o-identity-schema.json
slug: iot-events-s-s-o-identity
source_filename: iot-events-s-s-o-identity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-s-s-o-identity-schema.json\",\n  \"title\": \"SSOIdentity\",\n  \"description\": \"Contains information about your identity source in AWS Single Sign-On. For more information, see the <a href=\\\"https://docs.aws.amazon.com/singlesignon/latest/userguide/what-is.html\\\">AWS Single Sign-On User Guide</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The ID of the AWS SSO identity store.\"\n        }\n      ]\n    },\n    \"userId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SSOReferenceId\"\n        },\n        {\n          \"description\": \"The user ID.\"\n        }\n      ]\n  \
  \  }\n  },\n  \"required\": [\n    \"identityStoreId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-s-s-o-identity-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: SSOIdentity
---
