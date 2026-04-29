---
description: GetLogDeliveryConfigurationRequest schema from Amazon Cognito API
layout: schema
name: GetLogDeliveryConfigurationRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-log-delivery-configuration-request-schema.json
slug: user-pools-get-log-delivery-configuration-request
source_filename: user-pools-get-log-delivery-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-log-delivery-configuration-request-schema.json\",\n  \"title\": \"GetLogDeliveryConfigurationRequest\",\n  \"description\": \"GetLogDeliveryConfigurationRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The ID of the user pool where you want to view detailed activity logging configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-log-delivery-configuration-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetLogDeliveryConfigurationRequest
---
