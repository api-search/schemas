---
description: ''
layout: schema
name: Subscription
properties_list:
- description: The unique identifier for the subscription.
  name: id
  type: string
- description: The subject line of the subscription email.
  name: subject
  type: string
- description: Whether to attach an image of the view.
  name: attachImage
  type: boolean
- description: Whether to attach a PDF of the view.
  name: attachPdf
  type: boolean
- description: Custom message for the subscription.
  name: message
  type: string
- description: ''
  name: pageOrientation
  type: string
- description: ''
  name: pageSizeOption
  type: string
- description: Whether the subscription is suspended.
  name: suspended
  type: boolean
- description: ''
  name: content
  type: object
- description: ''
  name: schedule
  type: object
- description: ''
  name: user
  type: object
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-subscription-schema.json
slug: tableau-rest-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Subscription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the subscription.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject line of the subscription email.\"\n    },\n    \"attachImage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to attach an image of the view.\"\n    },\n    \"attachPdf\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to attach a PDF of the view.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Custom message for the subscription.\"\n    },\n    \"pageOrientation\": {\n      \"type\": \"string\"\n    },\n    \"pageSizeOption\": {\n      \"type\": \"string\"\n    },\n    \"suspended\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the subscription is suspended.\"\n    },\n    \"content\": {\n      \"type\": \"object\"\n    },\n    \"schedule\": {\n      \"type\": \"object\"\n    },\n    \"user\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-subscription-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Subscription
---
