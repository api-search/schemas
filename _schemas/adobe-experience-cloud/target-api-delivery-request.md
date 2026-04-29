---
description: DeliveryRequest schema
layout: schema
name: DeliveryRequest
properties_list:
- description: ''
  name: context
  type: object
- description: ''
  name: execute
  type: object
- description: ''
  name: prefetch
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/target-api-delivery-request-schema.json
slug: target-api-delivery-request
source_filename: target-api-delivery-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-delivery-request-schema.json\",\n  \"title\": \"DeliveryRequest\",\n  \"description\": \"DeliveryRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"context\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"channel\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"web\",\n            \"mobile\"\n          ]\n        },\n        \"userAgent\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"execute\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"mboxes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"index\"\
  : {\n                \"type\": \"integer\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"prefetch\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"views\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-delivery-request-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: DeliveryRequest
---
