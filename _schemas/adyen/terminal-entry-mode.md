---
description: EntryMode schema from Adyen API
layout: schema
name: EntryMode
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-entry-mode-schema.json
slug: terminal-entry-mode
source_filename: terminal-entry-mode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-entry-mode-schema.json\",\n  \"title\": \"EntryMode\",\n  \"description\": \"EntryMode schema from Adyen API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"Contactless\",\n      \"File\",\n      \"ICC\",\n      \"Keyed\",\n      \"MagStripe\",\n      \"Manual\",\n      \"Mobile\",\n      \"RFID\",\n      \"Scanned\",\n      \"SynchronousICC\",\n      \"Tapped\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-entry-mode-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: EntryMode
---
