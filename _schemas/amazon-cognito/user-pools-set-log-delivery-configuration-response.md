---
description: SetLogDeliveryConfigurationResponse schema from Amazon Cognito API
layout: schema
name: SetLogDeliveryConfigurationResponse
properties_list:
- description: ''
  name: LogDeliveryConfiguration
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-set-log-delivery-configuration-response-schema.json
slug: user-pools-set-log-delivery-configuration-response
source_filename: user-pools-set-log-delivery-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-set-log-delivery-configuration-response-schema.json\",\n  \"title\": \"SetLogDeliveryConfigurationResponse\",\n  \"description\": \"SetLogDeliveryConfigurationResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogDeliveryConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogDeliveryConfigurationType\"\n        },\n        {\n          \"description\": \"The detailed activity logging configuration that you applied to the requested user pool.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-set-log-delivery-configuration-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: SetLogDeliveryConfigurationResponse
---
