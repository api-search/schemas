---
description: CommonField schema from Adyen API
layout: schema
name: CommonField
properties_list:
- description: Name of the field. For example, Name of External Platform.
  name: name
  type: string
- description: Version of the field. For example, Version of External Platform.
  name: version
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-common-field-schema.json
slug: checkout-common-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-common-field-schema.json\",\n  \"title\": \"CommonField\",\n  \"description\": \"CommonField schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name of the field. For example, Name of External Platform.\",\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"description\": \"Version of the field. For example, Version of External Platform.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-common-field-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CommonField
---
