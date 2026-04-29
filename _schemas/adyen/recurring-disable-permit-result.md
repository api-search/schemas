---
description: DisablePermitResult schema from Adyen API
layout: schema
name: DisablePermitResult
properties_list:
- description: A unique reference associated with the request. This value is globally unique; quote it when communicating with us about this request.
  name: pspReference
  type: string
- description: Status of the disable request.
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-disable-permit-result-schema.json
slug: recurring-disable-permit-result
source_filename: recurring-disable-permit-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-disable-permit-result-schema.json\",\n  \"title\": \"DisablePermitResult\",\n  \"description\": \"DisablePermitResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pspReference\": {\n      \"description\": \"A unique reference associated with the request. This value is globally unique; quote it when communicating with us about this request.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"Status of the disable request.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-disable-permit-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DisablePermitResult
---
