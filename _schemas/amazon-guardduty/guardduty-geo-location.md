---
description: Contains information about the location of the remote IP address.
layout: schema
name: GeoLocation
properties_list:
- description: ''
  name: Lat
  type: object
- description: ''
  name: Lon
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-geo-location-schema.json
slug: guardduty-geo-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-geo-location-schema.json\",\n  \"title\": \"GeoLocation\",\n  \"description\": \"Contains information about the location of the remote IP address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Lat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lat\"\n          },\n          \"description\": \"The latitude information of the remote IP address.\"\n        }\n      ]\n    },\n    \"Lon\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lon\"\n          },\n          \"description\": \"The longitude information of the remote IP address.\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-geo-location-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GeoLocation
---
