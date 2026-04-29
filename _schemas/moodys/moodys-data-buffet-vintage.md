---
description: Metadata about a data vintage representing a historical revision of a series.
layout: schema
name: Vintage
properties_list:
- description: The date this vintage was published.
  name: vintageDate
  type: string
- description: Description of the vintage release context.
  name: description
  type: string
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-vintage-schema.json
slug: moodys-data-buffet-vintage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Vintage\",\n  \"type\": \"object\",\n  \"description\": \"Metadata about a data vintage representing a historical revision of a series.\",\n  \"properties\": {\n    \"vintageDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date this vintage was published.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the vintage release context.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-vintage-schema.json
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening
title: Vintage
---
