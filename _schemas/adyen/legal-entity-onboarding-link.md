---
description: OnboardingLink schema from Adyen API
layout: schema
name: OnboardingLink
properties_list:
- description: The URL of the hosted onboarding page where you need to redirect your user. This URL expires after 4 minutes and can only be used once. If the link expires, you need to create a new link.
  name: url
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-onboarding-link-schema.json
slug: legal-entity-onboarding-link
source_filename: legal-entity-onboarding-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-onboarding-link-schema.json\",\n  \"title\": \"OnboardingLink\",\n  \"description\": \"OnboardingLink schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"description\": \"The URL of the hosted onboarding page where you need to redirect your user. This URL expires after 4 minutes and can only be used once.\\n\\nIf the link expires, you need to create a new link.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-onboarding-link-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OnboardingLink
---
