---
description: ClassificationResultList schema from Avalara API
layout: schema
name: ClassificationResultList
properties_list:
- description: ''
  name: value
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/item-classification-classification-result-list-schema.json
slug: item-classification-classification-result-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-result-list-schema.json\",\n  \"title\": \"ClassificationResultList\",\n  \"description\": \"ClassificationResultList schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ClassificationResult\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-result-list-schema.json
tags:
- Taxes
title: ClassificationResultList
---
