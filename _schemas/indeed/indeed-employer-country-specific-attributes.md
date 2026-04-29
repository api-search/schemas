---
description: Country-scoped employer attributes. Provide an ISO 3166-1 two-letter country code to specify the country.
layout: schema
name: CountrySpecificAttributes
properties_list:
- description: ISO 3166-1 alpha-2 country code.
  name: country
  type: string
- description: The employer's website URL for this country.
  name: websiteUrl
  type: string
- description: The employer's contact phone number for this country.
  name: phoneNumber
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-country-specific-attributes-schema.json
slug: indeed-employer-country-specific-attributes
source_filename: indeed-employer-country-specific-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CountrySpecificAttributes\",\n  \"type\": \"object\",\n  \"description\": \"Country-scoped employer attributes. Provide an ISO 3166-1 two-letter country code to specify the country.\",\n  \"properties\": {\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code.\"\n    },\n    \"websiteUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The employer's website URL for this country.\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The employer's contact phone number for this country.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-country-specific-attributes-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: CountrySpecificAttributes
---
