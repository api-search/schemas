---
description: OnboardingThemes schema from Adyen API
layout: schema
name: OnboardingThemes
properties_list:
- description: The next page. Only present if there is a next page.
  name: next
  type: string
- description: The previous page. Only present if there is a previous page.
  name: previous
  type: string
- description: List of onboarding themes.
  name: themes
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-onboarding-themes-schema.json
slug: legal-entity-onboarding-themes
source_filename: legal-entity-onboarding-themes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-onboarding-themes-schema.json\",\n  \"title\": \"OnboardingThemes\",\n  \"description\": \"OnboardingThemes schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"next\": {\n      \"description\": \"The next page. Only present if there is a next page.\",\n      \"type\": \"string\"\n    },\n    \"previous\": {\n      \"description\": \"The previous page. Only present if there is a previous page.\",\n      \"type\": \"string\"\n    },\n    \"themes\": {\n      \"description\": \"List of onboarding themes.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/OnboardingTheme\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"themes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-onboarding-themes-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OnboardingThemes
---
