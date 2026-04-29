---
description: ErrorCondition schema from Adyen API
layout: schema
name: ErrorCondition
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-error-condition-schema.json
slug: terminal-error-condition
source_filename: terminal-error-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-error-condition-schema.json\",\n  \"title\": \"ErrorCondition\",\n  \"description\": \"ErrorCondition schema from Adyen API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Aborted\",\n    \"Busy\",\n    \"Cancel\",\n    \"DeviceOut\",\n    \"InProgress\",\n    \"InsertedCard\",\n    \"InvalidCard\",\n    \"LoggedOut\",\n    \"MessageFormat\",\n    \"NotAllowed\",\n    \"NotFound\",\n    \"PaymentRestriction\",\n    \"Refusal\",\n    \"UnavailableDevice\",\n    \"UnavailableService\",\n    \"UnreachableHost\",\n    \"WrongPIN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-error-condition-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ErrorCondition
---
