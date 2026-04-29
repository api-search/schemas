---
description: List of available API services.
layout: schema
name: ServicesResponse
properties_list:
- description: Array of available services.
  name: services
  type: array
provider_name: Biogen
provider_slug: biogen
schema_file: json-schema/biogen-services-response-schema.json
slug: biogen-services-response
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ServicesResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of available API services.\",\n  \"properties\": {\n    \"services\": {\n      \"type\": \"array\",\n      \"description\": \"Array of available services.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Service\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/json-schema/biogen-services-response-schema.json
tags:
- Biotechnology
- Healthcare
- Life Sciences
- Pharmaceuticals
- Neurology
title: ServicesResponse
---
