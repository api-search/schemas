---
description: It conveys Information related to the predefined message. Reference of a predefined message to display or print.
layout: schema
name: PredefinedContent
properties_list:
- description: Identification of a predefined message to display or print.
  name: ReferenceID
  type: string
- description: Identification of a language.
  name: Language
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-predefined-content-schema.json
slug: terminal-predefined-content
source_filename: terminal-predefined-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-predefined-content-schema.json\",\n  \"title\": \"PredefinedContent\",\n  \"description\": \"It conveys Information related to the predefined message. Reference of a predefined message to display or print.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReferenceID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Identification of a predefined message to display or print.\"\n    },\n    \"Language\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\",\n      \"description\": \"Identification of a language.\"\n    }\n  },\n  \"required\": [\n    \"ReferenceID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-predefined-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PredefinedContent
---
