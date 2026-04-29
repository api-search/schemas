---
description: OnboardingTheme schema from Adyen API
layout: schema
name: OnboardingTheme
properties_list:
- description: The creation date of the theme.
  name: createdAt
  type: string
- description: The description of the theme.
  name: description
  type: string
- description: The unique identifier of the theme.
  name: id
  type: string
- description: The properties of the theme.
  name: properties
  type: object
- description: The date when the theme was last updated.
  name: updatedAt
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-onboarding-theme-schema.json
slug: legal-entity-onboarding-theme
source_filename: legal-entity-onboarding-theme-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-onboarding-theme-schema.json\",\n  \"title\": \"OnboardingTheme\",\n  \"description\": \"OnboardingTheme schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"description\": \"The creation date of the theme.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"The description of the theme.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the theme.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The properties of the theme.\",\n      \"type\": \"object\"\n    },\n    \"updatedAt\": {\n      \"description\": \"The date\
  \ when the theme was last updated.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"properties\",\n    \"id\",\n    \"createdAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-onboarding-theme-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OnboardingTheme
---
