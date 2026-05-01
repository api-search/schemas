---
description: Result of a Veteran status confirmation request.
layout: schema
name: Veteran Confirmation
properties_list:
- description: ''
  name: veteran_status
  type: string
provider_name: Department of Veterans Affairs (VA)
provider_slug: department-of-veterans-affairs
schema_file: json-schema/va-veteran-confirmation-schema.json
slug: va-veteran-confirmation
source_filename: va-veteran-confirmation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-veterans-affairs/schemas/veteran-confirmation.json\",\n  \"title\": \"Veteran Confirmation\",\n  \"description\": \"Result of a Veteran status confirmation request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"veteran_status\": {\n      \"type\": \"string\",\n      \"enum\": [\"confirmed\", \"not confirmed\"]\n    }\n  },\n  \"required\": [\"veteran_status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-veterans-affairs/refs/heads/main/json-schema/va-veteran-confirmation-schema.json
tags:
- Federal Government
- Healthcare
- Veterans
title: Veteran Confirmation
---
