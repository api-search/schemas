---
description: ContactObject from WhatsApp API
layout: schema
name: ContactObject
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: addresses
  type: array
- description: Birthday in YYYY-MM-DD format
  name: birthday
  type: string
- description: ''
  name: emails
  type: array
- description: ''
  name: org
  type: object
- description: ''
  name: phones
  type: array
- description: ''
  name: urls
  type: array
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-contact-object-schema.json
slug: whatsapp-cloud-api-contact-object
source_filename: whatsapp-cloud-api-contact-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-contact-object-schema.json\",\n  \"title\": \"ContactObject\",\n  \"description\": \"ContactObject from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"formatted_name\"\n      ],\n      \"properties\": {\n        \"formatted_name\": {\n          \"type\": \"string\"\n        },\n        \"first_name\": {\n          \"type\": \"string\"\n        },\n        \"last_name\": {\n          \"type\": \"string\"\n        },\n        \"middle_name\": {\n          \"type\": \"string\"\n        },\n        \"prefix\": {\n          \"type\": \"string\"\n        },\n        \"suffix\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"items\"\
  : {\n        \"type\": \"object\",\n        \"properties\": {\n          \"street\": {\n            \"type\": \"string\"\n          },\n          \"city\": {\n            \"type\": \"string\"\n          },\n          \"state\": {\n            \"type\": \"string\"\n          },\n          \"zip\": {\n            \"type\": \"string\"\n          },\n          \"country\": {\n            \"type\": \"string\"\n          },\n          \"country_code\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HOME\",\n              \"WORK\"\n            ]\n          }\n        }\n      }\n    },\n    \"birthday\": {\n      \"type\": \"string\",\n      \"description\": \"Birthday in YYYY-MM-DD format\",\n      \"example\": \"example_value\"\n    },\n    \"emails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"email\": {\n     \
  \       \"type\": \"string\",\n            \"format\": \"email\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HOME\",\n              \"WORK\"\n            ]\n          }\n        }\n      }\n    },\n    \"org\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"company\": {\n          \"type\": \"string\"\n        },\n        \"department\": {\n          \"type\": \"string\"\n        },\n        \"title\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"phones\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"phone\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"CELL\",\n              \"MAIN\",\n              \"IPHONE\",\n              \"HOME\",\n              \"WORK\"\n            ]\n          },\n     \
  \     \"wa_id\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"urls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HOME\",\n              \"WORK\"\n            ]\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-contact-object-schema.json
tags: []
title: ContactObject
---
