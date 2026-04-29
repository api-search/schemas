---
description: Additional attributes for an employer, including both global and country-specific settings.
layout: schema
name: EmployerAttributes
properties_list:
- description: The type classification of the employer.
  name: employerType
  type: string
- description: Attributes that vary by country, such as website URLs, phone numbers, and locale-specific information.
  name: countrySpecificAttributes
  type: array
- description: Locale-specific employer attributes.
  name: localeSpecificAttributes
  type: array
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-employer-attributes-schema.json
slug: indeed-employer-employer-attributes
source_filename: indeed-employer-employer-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmployerAttributes\",\n  \"type\": \"object\",\n  \"description\": \"Additional attributes for an employer, including both global and country-specific settings.\",\n  \"properties\": {\n    \"employerType\": {\n      \"type\": \"string\",\n      \"description\": \"The type classification of the employer.\"\n    },\n    \"countrySpecificAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"Attributes that vary by country, such as website URLs, phone numbers, and locale-specific information.\"\n    },\n    \"localeSpecificAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"Locale-specific employer attributes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-employer-attributes-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: EmployerAttributes
---
