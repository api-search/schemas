---
description: An API product bundles API resources (proxies) for consumption by developers. Products define access control, quotas, and which API proxies and resources are available.
layout: schema
name: Apigee API Product
properties_list:
- description: Internal name of the API product. Must be unique within the organization.
  name: name
  type: string
- description: Name displayed in the developer portal.
  name: displayName
  type: string
- description: Description of the API product.
  name: description
  type: string
- description: How API keys are approved for the product.
  name: approvalType
  type: string
- description: Custom attributes for the API product (maximum 18).
  name: attributes
  type: array
- description: Environments where this product is available.
  name: environments
  type: array
- description: API proxies included in this product.
  name: proxies
  type: array
- description: OAuth scopes associated with the product.
  name: scopes
  type: array
- description: Number of requests permitted per quota interval.
  name: quota
  type: string
- description: Time interval over which the quota is applied.
  name: quotaInterval
  type: string
- description: Time unit for the quota interval.
  name: quotaTimeUnit
  type: string
- description: ''
  name: operationGroup
  type: object
- description: Output only. Unix time when the product was created.
  name: createdAt
  type: string
- description: Output only. Unix time when the product was last modified.
  name: lastModifiedAt
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-api-product-schema.json
slug: apigee-api-product
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/apigee/apigee-api-product-schema.json\",\n  \"title\": \"Apigee API Product\",\n  \"description\": \"An API product bundles API resources (proxies) for consumption by developers. Products define access control, quotas, and which API proxies and resources are available.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name of the API product. Must be unique within the organization.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Name displayed in the developer portal.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API product.\"\n    },\n    \"approvalType\": {\n      \"type\": \"string\",\n      \"description\": \"How API keys are approved for the product.\",\n      \"enum\": [\"manual\", \"auto\"\
  ]\n    },\n    \"attributes\": {\n      \"type\": \"array\",\n      \"description\": \"Custom attributes for the API product (maximum 18).\",\n      \"maxItems\": 18,\n      \"items\": {\n        \"$ref\": \"#/$defs/Attribute\"\n      }\n    },\n    \"environments\": {\n      \"type\": \"array\",\n      \"description\": \"Environments where this product is available.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"proxies\": {\n      \"type\": \"array\",\n      \"description\": \"API proxies included in this product.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"description\": \"OAuth scopes associated with the product.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"quota\": {\n      \"type\": \"string\",\n      \"description\": \"Number of requests permitted per quota interval.\"\n    },\n    \"quotaInterval\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Time interval over which the quota is applied.\"\n    },\n    \"quotaTimeUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Time unit for the quota interval.\",\n      \"enum\": [\"minute\", \"hour\", \"day\", \"month\"]\n    },\n    \"operationGroup\": {\n      \"$ref\": \"#/$defs/OperationGroup\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Unix time when the product was created.\",\n      \"readOnly\": true\n    },\n    \"lastModifiedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Unix time when the product was last modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"Attribute\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value pair used for custom attributes.\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"value\": { \"type\": \"string\" }\n      },\n      \"required\"\
  : [\"name\", \"value\"]\n    },\n    \"OperationGroup\": {\n      \"type\": \"object\",\n      \"description\": \"Groups operations for access control on an API product.\",\n      \"properties\": {\n        \"operationConfigs\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"apiSource\": { \"type\": \"string\" },\n              \"operations\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"resource\": { \"type\": \"string\" },\n                    \"methods\": {\n                      \"type\": \"array\",\n                      \"items\": { \"type\": \"string\" }\n                    }\n                  }\n                }\n              },\n              \"quota\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"limit\"\
  : { \"type\": \"string\" },\n                  \"interval\": { \"type\": \"string\" },\n                  \"timeUnit\": { \"type\": \"string\" }\n                }\n              }\n            }\n          }\n        },\n        \"operationConfigType\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/json-schema/apigee-api-product-schema.json
tags:
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Hybrid
- Integrations
- Microservices
- Monetization
title: Apigee API Product
---
