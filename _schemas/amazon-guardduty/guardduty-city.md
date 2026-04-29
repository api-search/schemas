---
description: Contains information about the city associated with the IP address.
layout: schema
name: City
properties_list:
- description: ''
  name: CityName
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-city-schema.json
slug: guardduty-city
source_filename: guardduty-city-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-city-schema.json\",\n  \"title\": \"City\",\n  \"description\": \"Contains information about the city associated with the IP address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CityName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cityName\"\n          },\n          \"description\": \"The city name of the remote IP address.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-city-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: City
---
