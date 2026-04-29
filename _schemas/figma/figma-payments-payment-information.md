---
description: An object describing a user's payment information for a plugin, widget, or Community file.
layout: schema
name: PaymentInformation
properties_list:
- description: The ID of the user whose payment information was queried. Can be used to verify the validity of a response.
  name: user_id
  type: string
- description: The ID of the plugin, widget, or Community file that was queried. Can be used to verify the validity of a response.
  name: resource_id
  type: string
- description: The type of the resource.
  name: resource_type
  type: string
- description: The UTC ISO 8601 timestamp indicating when the user purchased the resource. No value is given if the user has never purchased the resource.
  name: date_of_purchase
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-payments-payment-information-schema.json
slug: figma-payments-payment-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentInformation\",\n  \"type\": \"object\",\n  \"description\": \"An object describing a user's payment information for a plugin, widget, or Community file.\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the user whose payment information was queried. Can be used to verify the validity of a response.\"\n    },\n    \"resource_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the plugin, widget, or Community file that was queried. Can be used to verify the validity of a response.\"\n    },\n    \"resource_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource.\"\n    },\n    \"date_of_purchase\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 timestamp indicating when the user purchased the resource. No value is given if the user has never purchased\
  \ the resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-payments-payment-information-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: PaymentInformation
---
