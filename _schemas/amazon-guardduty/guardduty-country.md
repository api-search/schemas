---
description: Contains information about the country where the remote IP address is located.
layout: schema
name: Country
properties_list:
- description: ''
  name: CountryCode
  type: object
- description: ''
  name: CountryName
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-country-schema.json
slug: guardduty-country
source_filename: guardduty-country-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-country-schema.json\",\n  \"title\": \"Country\",\n  \"description\": \"Contains information about the country where the remote IP address is located.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CountryCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"countryCode\"\n          },\n          \"description\": \"The country code of the remote IP address.\"\n        }\n      ]\n    },\n    \"CountryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"countryName\"\n          },\n          \"description\": \"The country name of the remote IP address.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-country-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Country
---
