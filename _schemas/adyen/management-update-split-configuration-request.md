---
description: UpdateSplitConfigurationRequest schema from Adyen API
layout: schema
name: UpdateSplitConfigurationRequest
properties_list:
- description: Your description for the split configuration.
  name: description
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-update-split-configuration-request-schema.json
slug: management-update-split-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-split-configuration-request-schema.json\",\n  \"title\": \"UpdateSplitConfigurationRequest\",\n  \"description\": \"UpdateSplitConfigurationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Your description for the split configuration.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"description\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-split-configuration-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdateSplitConfigurationRequest
---
