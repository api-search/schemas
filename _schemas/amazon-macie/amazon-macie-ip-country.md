---
description: Provides information about the country that an IP address originated from.
layout: schema
name: IpCountry
properties_list:
- description: ''
  name: code
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-ip-country-schema.json
slug: amazon-macie-ip-country
source_filename: amazon-macie-ip-country-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-ip-country-schema.json\",\n  \"title\": \"IpCountry\",\n  \"description\": \"Provides information about the country that an IP address originated from.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The two-character code, in ISO 3166-1 alpha-2 format, for the country that the IP address originated from. For example, US for the United States.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the country that the IP address originated from.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-ip-country-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: IpCountry
---
