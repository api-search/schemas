---
description: Represents an Apigee organization, the top-level container for all Apigee resources including API proxies, products, developers, and environments.
layout: schema
name: Apigee Organization
properties_list:
- description: Output only. Name of the Apigee organization.
  name: name
  type: string
- description: Display name for the organization.
  name: displayName
  type: string
- description: Description of the organization.
  name: description
  type: string
- description: Output only. Project ID associated with the organization.
  name: projectId
  type: string
- description: Output only. Time the organization was created in milliseconds since epoch.
  name: createdAt
  type: string
- description: Output only. Time the organization was last modified in milliseconds since epoch.
  name: lastModifiedAt
  type: string
- description: Output only. Subscription type of the organization.
  name: subscriptionType
  type: string
- description: Output only. State of the organization.
  name: state
  type: string
- description: Required. Primary Google Cloud region for analytics data storage.
  name: analyticsRegion
  type: string
- description: Required. Runtime type of the Apigee organization.
  name: runtimeType
  type: string
- description: VPC network used for service networking.
  name: authorizedNetwork
  type: string
- description: Output only. List of environments in the organization.
  name: environments
  type: array
- description: Billing type of the organization.
  name: billingType
  type: string
- description: A collection of key-value property pairs.
  name: properties
  type: object
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-organization-schema.json
slug: apigee-organization
source_filename: apigee-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/apigee/apigee-organization-schema.json\",\n  \"title\": \"Apigee Organization\",\n  \"description\": \"Represents an Apigee organization, the top-level container for all Apigee resources including API proxies, products, developers, and environments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Name of the Apigee organization.\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the organization.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the organization.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Project ID associated with the organization.\",\n      \"readOnly\": true\n    },\n    \"createdAt\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Output only. Time the organization was created in milliseconds since epoch.\",\n      \"readOnly\": true\n    },\n    \"lastModifiedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Time the organization was last modified in milliseconds since epoch.\",\n      \"readOnly\": true\n    },\n    \"subscriptionType\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Subscription type of the organization.\",\n      \"readOnly\": true,\n      \"enum\": [\"SUBSCRIPTION_TYPE_UNSPECIFIED\", \"PAID\", \"TRIAL\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. State of the organization.\",\n      \"readOnly\": true,\n      \"enum\": [\"STATE_UNSPECIFIED\", \"CREATING\", \"ACTIVE\", \"DELETING\", \"UPDATING\"]\n    },\n    \"analyticsRegion\": {\n      \"type\": \"string\",\n      \"description\": \"Required. Primary Google Cloud region for analytics\
  \ data storage.\"\n    },\n    \"runtimeType\": {\n      \"type\": \"string\",\n      \"description\": \"Required. Runtime type of the Apigee organization.\",\n      \"enum\": [\"RUNTIME_TYPE_UNSPECIFIED\", \"CLOUD\", \"HYBRID\"]\n    },\n    \"authorizedNetwork\": {\n      \"type\": \"string\",\n      \"description\": \"VPC network used for service networking.\"\n    },\n    \"environments\": {\n      \"type\": \"array\",\n      \"description\": \"Output only. List of environments in the organization.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"billingType\": {\n      \"type\": \"string\",\n      \"description\": \"Billing type of the organization.\",\n      \"enum\": [\"BILLING_TYPE_UNSPECIFIED\", \"SUBSCRIPTION\", \"EVALUATION\", \"PAYG\"]\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"A collection of key-value property pairs.\",\n      \"properties\": {\n        \"property\": {\n    \
  \      \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"value\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"analyticsRegion\", \"runtimeType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/json-schema/apigee-organization-schema.json
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
title: Apigee Organization
---
