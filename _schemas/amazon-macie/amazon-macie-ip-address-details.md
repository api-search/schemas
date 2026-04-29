---
description: Provides information about the IP address of the device that an entity used to perform an action on an affected resource.
layout: schema
name: IpAddressDetails
properties_list:
- description: ''
  name: ipAddressV4
  type: object
- description: ''
  name: ipCity
  type: object
- description: ''
  name: ipCountry
  type: object
- description: ''
  name: ipGeoLocation
  type: object
- description: ''
  name: ipOwner
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-ip-address-details-schema.json
slug: amazon-macie-ip-address-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-ip-address-details-schema.json\",\n  \"title\": \"IpAddressDetails\",\n  \"description\": \"Provides information about the IP address of the device that an entity used to perform an action on an affected resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ipAddressV4\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Internet Protocol version 4 (IPv4) address of the device.\"\n        }\n      ]\n    },\n    \"ipCity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpCity\"\n        },\n        {\n          \"description\": \"The city that the IP address originated from.\"\n        }\n      ]\n    },\n    \"ipCountry\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/IpCountry\"\n        },\n        {\n          \"description\": \"The country that the IP address originated from.\"\n        }\n      ]\n    },\n    \"ipGeoLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGeoLocation\"\n        },\n        {\n          \"description\": \"The geographic coordinates of the location that the IP address originated from.\"\n        }\n      ]\n    },\n    \"ipOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpOwner\"\n        },\n        {\n          \"description\": \"The registered owner of the IP address.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-ip-address-details-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: IpAddressDetails
---
