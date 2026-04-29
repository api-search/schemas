---
description: InteractiveMessage from WhatsApp API
layout: schema
name: InteractiveMessage
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: header
  type: object
- description: ''
  name: body
  type: object
- description: ''
  name: footer
  type: object
- description: Action configuration varies by interactive type
  name: action
  type: object
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-interactive-message-schema.json
slug: whatsapp-cloud-api-interactive-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-interactive-message-schema.json\",\n  \"title\": \"InteractiveMessage\",\n  \"description\": \"InteractiveMessage from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"button\",\n        \"list\",\n        \"product\",\n        \"product_list\",\n        \"cta_url\",\n        \"location_request_message\",\n        \"flow\"\n      ],\n      \"example\": \"button\"\n    },\n    \"header\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"text\",\n            \"image\",\n            \"video\",\n            \"document\"\n          ]\n        },\n        \"text\": {\n          \"type\": \"string\"\n        },\n\
  \        \"image\": {\n          \"$ref\": \"#/components/schemas/MediaObject\"\n        },\n        \"video\": {\n          \"$ref\": \"#/components/schemas/MediaObject\"\n        },\n        \"document\": {\n          \"$ref\": \"#/components/schemas/DocumentObject\"\n        }\n      }\n    },\n    \"body\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"text\"\n      ],\n      \"properties\": {\n        \"text\": {\n          \"type\": \"string\",\n          \"maxLength\": 1024\n        }\n      }\n    },\n    \"footer\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"text\": {\n          \"type\": \"string\",\n          \"maxLength\": 60\n        }\n      }\n    },\n    \"action\": {\n      \"type\": \"object\",\n      \"description\": \"Action configuration varies by interactive type\",\n      \"properties\": {\n        \"buttons\": {\n          \"type\": \"array\",\n          \"maxItems\": 3,\n          \"items\": {\n            \"type\": \"\
  object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"reply\"\n                ]\n              },\n              \"reply\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"maxLength\": 256\n                  },\n                  \"title\": {\n                    \"type\": \"string\",\n                    \"maxLength\": 20\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"button\": {\n          \"type\": \"string\",\n          \"description\": \"Button text for list messages\",\n          \"maxLength\": 20\n        },\n        \"sections\": {\n          \"type\": \"array\",\n          \"maxItems\": 10,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/ListSection\"\n          }\n      \
  \  },\n        \"catalog_id\": {\n          \"type\": \"string\"\n        },\n        \"product_retailer_id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Action name for CTA URL or flow messages\"\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"description\": \"Parameters for CTA URL or flow actions\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-interactive-message-schema.json
tags: []
title: InteractiveMessage
---
