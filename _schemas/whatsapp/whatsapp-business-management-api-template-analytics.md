---
description: TemplateAnalytics from WhatsApp API
layout: schema
name: TemplateAnalytics
properties_list:
- description: ''
  name: template_analytics
  type: object
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-business-management-api-template-analytics-schema.json
slug: whatsapp-business-management-api-template-analytics
source_filename: whatsapp-business-management-api-template-analytics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-template-analytics-schema.json\",\n  \"title\": \"TemplateAnalytics\",\n  \"description\": \"TemplateAnalytics from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"template_analytics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"template_id\": {\n                \"type\": \"string\"\n              },\n              \"data_points\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"start\": {\n                      \"type\": \"integer\"\n                    },\n      \
  \              \"end\": {\n                      \"type\": \"integer\"\n                    },\n                    \"sent\": {\n                      \"type\": \"integer\"\n                    },\n                    \"delivered\": {\n                      \"type\": \"integer\"\n                    },\n                    \"read\": {\n                      \"type\": \"integer\"\n                    },\n                    \"clicked\": {\n                      \"type\": \"integer\"\n                    },\n                    \"cost\": {\n                      \"type\": \"number\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-template-analytics-schema.json
tags: []
title: TemplateAnalytics
---
