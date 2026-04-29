---
description: The location of the job.
layout: schema
name: JobLocation
properties_list:
- description: Street address of the job location.
  name: streetAddress
  type: string
- description: City where the job is located.
  name: city
  type: string
- description: State, province, or region.
  name: state
  type: string
- description: Postal or ZIP code.
  name: postalCode
  type: string
- description: ISO 3166-1 alpha-2 country code.
  name: country
  type: string
- description: A human-readable formatted address string.
  name: formattedAddress
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-job-location-schema.json
slug: indeed-employer-job-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobLocation\",\n  \"type\": \"object\",\n  \"description\": \"The location of the job.\",\n  \"properties\": {\n    \"streetAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Street address of the job location.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City where the job is located.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State, province, or region.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code.\"\n    },\n    \"formattedAddress\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable formatted address string.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-job-location-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: JobLocation
---
