---
description: DeliveryResponse schema
layout: schema
name: DeliveryResponse
properties_list:
- description: ''
  name: requestId
  type: string
- description: ''
  name: execute
  type: object
- description: ''
  name: prefetch
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/target-api-delivery-response-schema.json
slug: target-api-delivery-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-delivery-response-schema.json\",\n  \"title\": \"DeliveryResponse\",\n  \"description\": \"DeliveryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\"\n    },\n    \"execute\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"mboxes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"options\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"type\": {\n                      \"type\": \"string\"\n                \
  \    },\n                    \"content\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"prefetch\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-delivery-response-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: DeliveryResponse
---
