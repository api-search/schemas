---
description: GetSubscriptionResponse schema from Amazon CodeCatalyst
layout: schema
name: GetSubscriptionResponse
properties_list:
- description: ''
  name: subscriptionType
  type: object
- description: ''
  name: awsAccountName
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-get-subscription-response-schema.json
slug: amazon-codecatalyst-get-subscription-response
source_filename: amazon-codecatalyst-get-subscription-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-get-subscription-response-schema.json\",\n  \"title\": \"GetSubscriptionResponse\",\n  \"description\": \"GetSubscriptionResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscriptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of the billing plan for the space.\"\n        }\n      ]\n    },\n    \"awsAccountName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The display name of the Amazon Web Services account used for billing for the space.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-get-subscription-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: GetSubscriptionResponse
---
