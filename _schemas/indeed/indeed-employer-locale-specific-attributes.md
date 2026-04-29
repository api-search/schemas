---
description: Locale-specific employer attributes for multilingual support.
layout: schema
name: LocaleSpecificAttributes
properties_list:
- description: IETF BCP 47 language tag.
  name: locale
  type: string
- description: Localized employer name.
  name: employerName
  type: string
- description: Localized employer description.
  name: employerDescription
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-locale-specific-attributes-schema.json
slug: indeed-employer-locale-specific-attributes
source_filename: indeed-employer-locale-specific-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LocaleSpecificAttributes\",\n  \"type\": \"object\",\n  \"description\": \"Locale-specific employer attributes for multilingual support.\",\n  \"properties\": {\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"IETF BCP 47 language tag.\"\n    },\n    \"employerName\": {\n      \"type\": \"string\",\n      \"description\": \"Localized employer name.\"\n    },\n    \"employerDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Localized employer description.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-locale-specific-attributes-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: LocaleSpecificAttributes
---
