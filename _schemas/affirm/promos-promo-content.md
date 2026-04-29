---
description: Promotional messaging content including ALA text and modal content.
layout: schema
name: PromoContent
properties_list:
- description: Plain text "as low as" monthly payment message, suitable for inline display on product and cart pages.
  name: ala
  type: string
- description: HTML-formatted "as low as" monthly payment message with appropriate markup for web display.
  name: html_ala
  type: string
- description: Modal headline text displayed at the top of the Affirm educational modal.
  name: headline
  type: string
- description: Modal tagline or subheading text.
  name: tagline
  type: string
- description: Call-to-action button label text for the modal.
  name: button
  type: string
- description: HTML-formatted legal disclosure footer for the modal.
  name: html_footer
  type: string
- description: Full description text for the educational modal explaining Affirm financing.
  name: description
  type: string
- description: ''
  name: config
  type: object
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/promos-promo-content-schema.json
slug: promos-promo-content
source_filename: promos-promo-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/promos-promo-content-schema.json\",\n  \"title\": \"PromoContent\",\n  \"description\": \"Promotional messaging content including ALA text and modal content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ala\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text \\\"as low as\\\" monthly payment message, suitable for inline display on product and cart pages.\",\n      \"example\": \"example_value\"\n    },\n    \"html_ala\": {\n      \"type\": \"string\",\n      \"description\": \"HTML-formatted \\\"as low as\\\" monthly payment message with appropriate markup for web display.\",\n      \"example\": \"example_value\"\n    },\n    \"headline\": {\n      \"type\": \"string\",\n      \"description\": \"Modal headline text displayed at the top of the Affirm educational modal.\",\n      \"\
  example\": \"example_value\"\n    },\n    \"tagline\": {\n      \"type\": \"string\",\n      \"description\": \"Modal tagline or subheading text.\",\n      \"example\": \"example_value\"\n    },\n    \"button\": {\n      \"type\": \"string\",\n      \"description\": \"Call-to-action button label text for the modal.\",\n      \"example\": \"example_value\"\n    },\n    \"html_footer\": {\n      \"type\": \"string\",\n      \"description\": \"HTML-formatted legal disclosure footer for the modal.\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Full description text for the educational modal explaining Affirm financing.\",\n      \"example\": \"Example description text\"\n    },\n    \"config\": {\n      \"$ref\": \"#/components/schemas/PromoConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/promos-promo-content-schema.json
tags: []
title: PromoContent
---
