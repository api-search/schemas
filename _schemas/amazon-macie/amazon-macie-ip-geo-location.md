---
description: Provides geographic coordinates that indicate where a specified IP address originated from.
layout: schema
name: IpGeoLocation
properties_list:
- description: ''
  name: lat
  type: object
- description: ''
  name: lon
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-ip-geo-location-schema.json
slug: amazon-macie-ip-geo-location
source_filename: amazon-macie-ip-geo-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-ip-geo-location-schema.json\",\n  \"title\": \"IpGeoLocation\",\n  \"description\": \"Provides geographic coordinates that indicate where a specified IP address originated from.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"description\": \"The latitude coordinate of the location, rounded to four decimal places.\"\n        }\n      ]\n    },\n    \"lon\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"description\": \"The longitude coordinate of the location, rounded to four decimal places.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-ip-geo-location-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: IpGeoLocation
---
