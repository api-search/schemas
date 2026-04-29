---
description: The logging parameters of a user pool.
layout: schema
name: LogDeliveryConfigurationType
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: LogConfigurations
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-log-delivery-configuration-type-schema.json
slug: user-pools-log-delivery-configuration-type
source_filename: user-pools-log-delivery-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-log-delivery-configuration-type-schema.json\",\n  \"title\": \"LogDeliveryConfigurationType\",\n  \"description\": \"The logging parameters of a user pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The ID of the user pool where you configured detailed activity logging.\"\n        }\n      ]\n    },\n    \"LogConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogConfigurationListType\"\n        },\n        {\n          \"description\": \"The detailed activity logging destination of a user pool.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"LogConfigurations\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-log-delivery-configuration-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: LogDeliveryConfigurationType
---
