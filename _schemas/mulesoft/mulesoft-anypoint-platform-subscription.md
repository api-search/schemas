---
description: Subscription plan details for the organization
layout: schema
name: Subscription
properties_list:
- description: Subscription category
  name: category
  type: string
- description: Subscription type
  name: type
  type: string
- description: Subscription expiration date
  name: expiration
  type: string
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-subscription-schema.json
slug: mulesoft-anypoint-platform-subscription
source_filename: mulesoft-anypoint-platform-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Subscription\",\n  \"type\": \"object\",\n  \"description\": \"Subscription plan details for the organization\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription category\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription type\"\n    },\n    \"expiration\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription expiration date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-subscription-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: Subscription
---
