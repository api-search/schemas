---
description: DescribeRiskConfigurationResponse schema from Amazon Cognito API
layout: schema
name: DescribeRiskConfigurationResponse
properties_list:
- description: ''
  name: RiskConfiguration
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-describe-risk-configuration-response-schema.json
slug: user-pools-describe-risk-configuration-response
source_filename: user-pools-describe-risk-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-risk-configuration-response-schema.json\",\n  \"title\": \"DescribeRiskConfigurationResponse\",\n  \"description\": \"DescribeRiskConfigurationResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RiskConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RiskConfigurationType\"\n        },\n        {\n          \"description\": \"The risk configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RiskConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-risk-configuration-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DescribeRiskConfigurationResponse
---
