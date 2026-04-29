---
description: CreateDomainRequest schema from AhaSend API
layout: schema
name: CreateDomainRequest
properties_list:
- description: Fully qualified domain name
  name: domain
  type: string
- description: DKIM Private Key for the domain. Only RSA keys with a minimum key size of 2048 bits are supported. **Note:** This parameter is only supported on [Platform Partner](https://ahasend.com/partners) accoun
  name: dkim_private_key
  type: string
- description: Optional custom tracking subdomain. Omit to use the default on create.
  name: tracking_subdomain
  type: string
- description: Optional custom return-path subdomain. Omit to use the default on create.
  name: return_path_subdomain
  type: string
- description: Optional custom subscription management subdomain. Omit to use the default on create.
  name: subscription_subdomain
  type: string
- description: Optional custom media subdomain. Omit to use the default on create.
  name: media_subdomain
  type: string
- description: Optional custom DKIM rotation interval in days. Only supported for managed DNS domains on eligible plans.
  name: dkim_rotation_interval_days
  type: integer
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-create-domain-request-schema.json
slug: openapi-v2-create-domain-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-domain-request-schema.json\",\n  \"title\": \"CreateDomainRequest\",\n  \"description\": \"CreateDomainRequest schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"format\": \"hostname\",\n      \"description\": \"Fully qualified domain name\",\n      \"example\": \"mail.example.com\"\n    },\n    \"dkim_private_key\": {\n      \"type\": \"string\",\n      \"description\": \"DKIM Private Key for the domain. Only RSA keys with a minimum key size of 2048 bits are supported.\\n\\n**Note:** This parameter is only supported on [Platform Partner](https://ahasend.com/partners) accounts.\\n\",\n      \"example\": \"aha-sk-aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\"\n    },\n    \"tracking_subdomain\": {\n   \
  \   \"type\": \"string\",\n      \"description\": \"Optional custom tracking subdomain. Omit to use the default on create.\",\n      \"example\": \"mail.example.com\"\n    },\n    \"return_path_subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"Optional custom return-path subdomain. Omit to use the default on create.\",\n      \"example\": \"mail.example.com\"\n    },\n    \"subscription_subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"Optional custom subscription management subdomain. Omit to use the default on create.\",\n      \"example\": \"mail.example.com\"\n    },\n    \"media_subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"Optional custom media subdomain. Omit to use the default on create.\",\n      \"example\": \"mail.example.com\"\n    },\n    \"dkim_rotation_interval_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Optional custom DKIM rotation interval in days. Only supported for managed DNS domains\
  \ on eligible plans.\",\n      \"example\": 1\n    }\n  },\n  \"required\": [\n    \"domain\"\n  ],\n  \"example\": {\n    \"domain\": \"example.com\",\n    \"tracking_subdomain\": \"click\",\n    \"return_path_subdomain\": \"mail\",\n    \"subscription_subdomain\": \"preferences\",\n    \"media_subdomain\": \"media\",\n    \"dkim_rotation_interval_days\": 45\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-domain-request-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: CreateDomainRequest
---
