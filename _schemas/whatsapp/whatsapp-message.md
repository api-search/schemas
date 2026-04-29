---
description: Schema for outbound WhatsApp messages sent via the Cloud API POST /{phone-number-id}/messages endpoint. Covers all message types including text, media, location, contacts, interactive, template, and reaction messages.
layout: schema
name: WhatsApp Message
properties_list:
- description: Must be 'whatsapp'
  name: messaging_product
  type: string
- description: Recipient type, currently only 'individual' is supported
  name: recipient_type
  type: string
- description: Recipient phone number in E.164 format without the leading +
  name: to
  type: string
- description: Message type
  name: type
  type: string
- description: ''
  name: context
  type: object
- description: Arbitrary string for tracking, included in webhook delivery
  name: biz_opaque_callback_data
  type: string
- description: ''
  name: text
  type: object
- description: ''
  name: image
  type: object
- description: ''
  name: video
  type: object
- description: ''
  name: audio
  type: object
- description: ''
  name: document
  type: object
- description: ''
  name: sticker
  type: object
- description: ''
  name: location
  type: object
- description: Array of contact cards to send
  name: contacts
  type: array
- description: ''
  name: interactive
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: reaction
  type: object
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-message-schema.json
slug: whatsapp-message
source_filename: whatsapp-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developers.facebook.com/schemas/whatsapp/message.json\",\n  \"title\": \"WhatsApp Message\",\n  \"description\": \"Schema for outbound WhatsApp messages sent via the Cloud API POST /{phone-number-id}/messages endpoint. Covers all message types including text, media, location, contacts, interactive, template, and reaction messages.\",\n  \"type\": \"object\",\n  \"required\": [\"messaging_product\", \"to\", \"type\"],\n  \"properties\": {\n    \"messaging_product\": {\n      \"type\": \"string\",\n      \"const\": \"whatsapp\",\n      \"description\": \"Must be 'whatsapp'\"\n    },\n    \"recipient_type\": {\n      \"type\": \"string\",\n      \"default\": \"individual\",\n      \"description\": \"Recipient type, currently only 'individual' is supported\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"Recipient phone number in E.164 format without the leading\
  \ +\",\n      \"pattern\": \"^[1-9]\\\\d{1,14}$\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"text\", \"image\", \"video\", \"audio\", \"document\", \"sticker\", \"location\", \"contacts\", \"interactive\", \"template\", \"reaction\"],\n      \"description\": \"Message type\"\n    },\n    \"context\": {\n      \"$ref\": \"#/$defs/Context\"\n    },\n    \"biz_opaque_callback_data\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary string for tracking, included in webhook delivery\"\n    },\n    \"text\": {\n      \"$ref\": \"#/$defs/TextMessage\"\n    },\n    \"image\": {\n      \"$ref\": \"#/$defs/MediaMessage\"\n    },\n    \"video\": {\n      \"$ref\": \"#/$defs/MediaMessage\"\n    },\n    \"audio\": {\n      \"$ref\": \"#/$defs/AudioMessage\"\n    },\n    \"document\": {\n      \"$ref\": \"#/$defs/DocumentMessage\"\n    },\n    \"sticker\": {\n      \"$ref\": \"#/$defs/StickerMessage\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/LocationMessage\"\
  \n    },\n    \"contacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Contact\"\n      },\n      \"description\": \"Array of contact cards to send\"\n    },\n    \"interactive\": {\n      \"$ref\": \"#/$defs/InteractiveMessage\"\n    },\n    \"template\": {\n      \"$ref\": \"#/$defs/TemplateMessage\"\n    },\n    \"reaction\": {\n      \"$ref\": \"#/$defs/ReactionMessage\"\n    }\n  },\n  \"$defs\": {\n    \"Context\": {\n      \"type\": \"object\",\n      \"description\": \"Context for reply messages\",\n      \"required\": [\"message_id\"],\n      \"properties\": {\n        \"message_id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the message being replied to\"\n        }\n      }\n    },\n    \"TextMessage\": {\n      \"type\": \"object\",\n      \"required\": [\"body\"],\n      \"properties\": {\n        \"body\": {\n          \"type\": \"string\",\n          \"maxLength\": 4096,\n          \"description\": \"Message\
  \ text content\"\n        },\n        \"preview_url\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Set true to render URL previews\"\n        }\n      }\n    },\n    \"MediaMessage\": {\n      \"type\": \"object\",\n      \"description\": \"Image or video message. Provide either id (for uploaded media) or link (for URL-hosted media), not both.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Media ID from a previous upload\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"HTTPS URL of the media file\"\n        },\n        \"caption\": {\n          \"type\": \"string\",\n          \"maxLength\": 1024,\n          \"description\": \"Caption text\"\n        }\n      }\n    },\n    \"AudioMessage\": {\n      \"type\": \"object\",\n      \"description\": \"Audio message. Supported formats: AAC, MP4, MPEG,\
  \ AMR, OGG (OPUS). Max 16 MB.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Media ID from a previous upload\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"HTTPS URL of the audio file\"\n        }\n      }\n    },\n    \"DocumentMessage\": {\n      \"type\": \"object\",\n      \"description\": \"Document message. Max 100 MB.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Media ID from a previous upload\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"HTTPS URL of the document\"\n        },\n        \"caption\": {\n          \"type\": \"string\",\n          \"description\": \"Caption text\"\n        },\n        \"filename\": {\n          \"type\": \"string\",\n          \"description\": \"Filename to display\
  \ to recipient\"\n        }\n      }\n    },\n    \"StickerMessage\": {\n      \"type\": \"object\",\n      \"description\": \"Sticker message. WebP format only. Max 100 KB (static), 500 KB (animated).\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    },\n    \"LocationMessage\": {\n      \"type\": \"object\",\n      \"required\": [\"latitude\", \"longitude\"],\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Location name\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Location\
  \ address\"\n        }\n      }\n    },\n    \"Contact\": {\n      \"type\": \"object\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"object\",\n          \"required\": [\"formatted_name\"],\n          \"properties\": {\n            \"formatted_name\": {\n              \"type\": \"string\"\n            },\n            \"first_name\": {\n              \"type\": \"string\"\n            },\n            \"last_name\": {\n              \"type\": \"string\"\n            },\n            \"middle_name\": {\n              \"type\": \"string\"\n            },\n            \"prefix\": {\n              \"type\": \"string\"\n            },\n            \"suffix\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"addresses\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"street\": { \"type\": \"string\" },\n  \
  \            \"city\": { \"type\": \"string\" },\n              \"state\": { \"type\": \"string\" },\n              \"zip\": { \"type\": \"string\" },\n              \"country\": { \"type\": \"string\" },\n              \"country_code\": { \"type\": \"string\" },\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"HOME\", \"WORK\"]\n              }\n            }\n          }\n        },\n        \"birthday\": {\n          \"type\": \"string\",\n          \"pattern\": \"^\\\\d{4}-\\\\d{2}-\\\\d{2}$\",\n          \"description\": \"Birthday in YYYY-MM-DD format\"\n        },\n        \"emails\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"email\": {\n                \"type\": \"string\",\n                \"format\": \"email\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"HOME\", \"\
  WORK\"]\n              }\n            }\n          }\n        },\n        \"org\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"company\": { \"type\": \"string\" },\n            \"department\": { \"type\": \"string\" },\n            \"title\": { \"type\": \"string\" }\n          }\n        },\n        \"phones\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"phone\": { \"type\": \"string\" },\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"CELL\", \"MAIN\", \"IPHONE\", \"HOME\", \"WORK\"]\n              },\n              \"wa_id\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"urls\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"url\": {\n                \"type\": \"string\",\n          \
  \      \"format\": \"uri\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"HOME\", \"WORK\"]\n              }\n            }\n          }\n        }\n      }\n    },\n    \"InteractiveMessage\": {\n      \"type\": \"object\",\n      \"required\": [\"type\", \"action\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"button\", \"list\", \"product\", \"product_list\", \"cta_url\", \"location_request_message\", \"flow\"]\n        },\n        \"header\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\"text\", \"image\", \"video\", \"document\"]\n            },\n            \"text\": { \"type\": \"string\" }\n          }\n        },\n        \"body\": {\n          \"type\": \"object\",\n          \"required\": [\"text\"],\n          \"properties\": {\n            \"\
  text\": {\n              \"type\": \"string\",\n              \"maxLength\": 1024\n            }\n          }\n        },\n        \"footer\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"text\": {\n              \"type\": \"string\",\n              \"maxLength\": 60\n            }\n          }\n        },\n        \"action\": {\n          \"type\": \"object\",\n          \"description\": \"Action configuration varies by interactive type\"\n        }\n      }\n    },\n    \"TemplateMessage\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"language\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Template name\"\n        },\n        \"language\": {\n          \"type\": \"object\",\n          \"required\": [\"code\"],\n          \"properties\": {\n            \"code\": {\n              \"type\": \"string\",\n              \"description\": \"Language/locale code (e.g., en_US)\"\
  \n            },\n            \"policy\": {\n              \"type\": \"string\",\n              \"default\": \"deterministic\"\n            }\n          }\n        },\n        \"components\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\"type\"],\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"header\", \"body\", \"button\"]\n              },\n              \"sub_type\": {\n                \"type\": \"string\",\n                \"enum\": [\"quick_reply\", \"url\", \"copy_code\", \"flow\", \"catalog\"]\n              },\n              \"index\": {\n                \"type\": \"string\"\n              },\n              \"parameters\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"required\": [\"type\"],\n                  \"properties\": {\n         \
  \           \"type\": {\n                      \"type\": \"string\",\n                      \"enum\": [\"text\", \"image\", \"video\", \"document\", \"location\", \"currency\", \"date_time\", \"payload\", \"coupon_code\"]\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"ReactionMessage\": {\n      \"type\": \"object\",\n      \"required\": [\"message_id\", \"emoji\"],\n      \"properties\": {\n        \"message_id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the message to react to\"\n        },\n        \"emoji\": {\n          \"type\": \"string\",\n          \"description\": \"Emoji character or empty string to remove reaction\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-message-schema.json
tags: []
title: WhatsApp Message
---
