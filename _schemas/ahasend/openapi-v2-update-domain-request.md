---
description: UpdateDomainRequest schema from AhaSend API
layout: schema
name: UpdateDomainRequest
properties_list:
- description: Optional custom tracking subdomain. Omit to leave the current value unchanged.
  name: tracking_subdomain
  type: string
- description: Optional custom return-path subdomain. Omit to leave the current value unchanged.
  name: return_path_subdomain
  type: string
- description: Optional custom subscription management subdomain. Omit to leave the current value unchanged.
  name: subscription_subdomain
  type: string
- description: Optional custom media subdomain. Omit to leave the current value unchanged.
  name: media_subdomain
  type: string
- description: Optional custom DKIM rotation interval in days. Omit to leave the current value unchanged. Only supported for managed DNS domains on eligible plans.
  name: dkim_rotation_interval_days
  type: integer
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-update-domain-request-schema.json
slug: openapi-v2-update-domain-request
source_filename: openapi-v2-update-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-update-domain-request-schema.json\",\n  \"title\": \"UpdateDomainRequest\",\n  \"description\": \"UpdateDomainRequest schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tracking_subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"Optional custom tracking subdomain. Omit to leave the current value unchanged.\",\n      \"example\": \"mail.example.com\"\n    },\n    \"return_path_subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"Optional custom return-path subdomain. Omit to leave the current value unchanged.\",\n      \"example\": \"mail.example.com\"\n    },\n    \"subscription_subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"Optional custom subscription management subdomain. Omit to leave the current value unchanged.\"\
  ,\n      \"example\": \"mail.example.com\"\n    },\n    \"media_subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"Optional custom media subdomain. Omit to leave the current value unchanged.\",\n      \"example\": \"mail.example.com\"\n    },\n    \"dkim_rotation_interval_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Optional custom DKIM rotation interval in days. Omit to leave the current value unchanged. Only supported for managed DNS domains on eligible plans.\",\n      \"example\": 1\n    }\n  },\n  \"example\": {\n    \"tracking_subdomain\": \"click\",\n    \"return_path_subdomain\": \"mail\",\n    \"subscription_subdomain\": \"preferences\",\n    \"media_subdomain\": \"media\",\n    \"dkim_rotation_interval_days\": 45\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-update-domain-request-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: UpdateDomainRequest
---
