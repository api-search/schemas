---
description: A subscription is the product that allows for applications to be hosted with Acquia. In addition, a subscription grants access to various additional services.
layout: schema
name: Subscription
properties_list:
- description: The subscription ID.
  name: id
  type: integer
- description: The subscription UUID.
  name: uuid
  type: string
- description: The subscription name.
  name: name
  type: string
- description: The time when the service defined by the subscription becomes available.
  name: start_at
  type: string
- description: The time when the service expires.
  name: expire_at
  type: string
- description: Defines the type of service this subscription is entitled to.
  name: product
  type: object
- description: The number of applications this subscription is entitled to.
  name: applications_total
  type: integer
- description: The number of applications used.
  name: applications_used
  type: integer
- description: ''
  name: organization
  type: object
- description: ''
  name: flags
  type: object
- description: ''
  name: _links
  type: object
- description: A collection of resources related to the subscription.
  name: _embedded
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-subscription-schema.json
slug: acquia-cloud-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-subscription-schema.json\",\n  \"title\": \"Subscription\",\n  \"description\": \"A subscription is the product that allows for applications to be hosted with Acquia.\\nIn addition, a subscription grants access to various additional services.\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The subscription ID.\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription UUID.\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription name.\"\n    },\n    \"start_at\": {\n      \"type\": \"string\",\n      \"description\": \"The time when the service defined by the subscription becomes available.\"\n    },\n    \"expire_at\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The time when the service expires.\"\n    },\n    \"product\": {\n      \"type\": \"object\",\n      \"description\": \"Defines the type of service this subscription is entitled to.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The product ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The product name.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The product type.\"\n        }\n      }\n    },\n    \"applications_total\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of applications this subscription is entitled to.\"\n    },\n    \"applications_used\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of applications used.\"\n    },\n    \"organization\": {\n      \"type\": \"object\",\n      \"deprecated\": true,\n\
  \      \"required\": [\n        \"uuid\",\n        \"name\"\n      ],\n      \"properties\": {\n        \"uuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The organization's UUID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The human-readable organization name.\"\n        }\n      }\n    },\n    \"flags\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_subscription-flags\"\n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    },\n    \"_embedded\": {\n      \"type\": \"object\",\n      \"description\": \"A collection of resources related to the subscription.\",\n      \"properties\": {\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_organization-stub\"\n          }\n        }\n      }\n   \
  \ }\n  },\n  \"required\": [\n    \"id\",\n    \"uuid\",\n    \"name\",\n    \"start_at\",\n    \"expire_at\",\n    \"product\",\n    \"applications_total\",\n    \"applications_used\",\n    \"organization\",\n    \"flags\",\n    \"_links\",\n    \"_embedded\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-subscription-schema.json
tags:
- Content
- Experience
title: Subscription
---
