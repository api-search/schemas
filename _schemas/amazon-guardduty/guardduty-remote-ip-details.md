---
description: Contains information about the remote IP address of the connection.
layout: schema
name: RemoteIpDetails
properties_list:
- description: ''
  name: City
  type: object
- description: ''
  name: Country
  type: object
- description: ''
  name: GeoLocation
  type: object
- description: ''
  name: IpAddressV4
  type: object
- description: ''
  name: Organization
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-remote-ip-details-schema.json
slug: guardduty-remote-ip-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-remote-ip-details-schema.json\",\n  \"title\": \"RemoteIpDetails\",\n  \"description\": \"Contains information about the remote IP address of the connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"City\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/City\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"city\"\n          },\n          \"description\": \"The city information of the remote IP address.\"\n        }\n      ]\n    },\n    \"Country\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Country\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"country\"\n          },\n          \"description\": \"The country code of the remote IP address.\"\n        }\n      ]\n  \
  \  },\n    \"GeoLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeoLocation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"geoLocation\"\n          },\n          \"description\": \"The location information of the remote IP address.\"\n        }\n      ]\n    },\n    \"IpAddressV4\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ipAddressV4\"\n          },\n          \"description\": \"The IPv4 remote address of the connection.\"\n        }\n      ]\n    },\n    \"Organization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Organization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"organization\"\n          },\n          \"description\": \"The ISP organization information of the remote IP address.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-remote-ip-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: RemoteIpDetails
---
