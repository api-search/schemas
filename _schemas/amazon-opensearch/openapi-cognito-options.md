---
description: Options to specify the Cognito user and identity pools for Kibana authentication. For more information, see <a href="http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-cognito-auth.html" target="_blank">Amazon Cognito Authentication for Kibana</a>.
layout: schema
name: CognitoOptions
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: RoleArn
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-cognito-options-schema.json
slug: openapi-cognito-options
source_filename: openapi-cognito-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-cognito-options-schema.json\",\n  \"title\": \"CognitoOptions\",\n  \"description\": \"Options to specify the Cognito user and identity pools for Kibana authentication. For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-cognito-auth.html\\\" target=\\\"_blank\\\">Amazon Cognito Authentication for Kibana</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies the option to enable Cognito for Kibana authentication.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolId\"\n        },\n    \
  \    {\n          \"description\": \"Specifies the Cognito user pool ID for Kibana authentication.\"\n        }\n      ]\n    },\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"Specifies the Cognito identity pool ID for Kibana authentication.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"Specifies the role ARN that provides Elasticsearch permissions for accessing Cognito resources.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-cognito-options-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: CognitoOptions
---
