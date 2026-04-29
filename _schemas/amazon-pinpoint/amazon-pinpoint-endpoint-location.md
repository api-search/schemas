---
description: Specifies geographic information about an endpoint.
layout: schema
name: EndpointLocation
properties_list:
- description: ''
  name: City
  type: object
- description: ''
  name: Country
  type: object
- description: ''
  name: Latitude
  type: object
- description: ''
  name: Longitude
  type: object
- description: ''
  name: PostalCode
  type: object
- description: ''
  name: Region
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-endpoint-location-schema.json
slug: amazon-pinpoint-endpoint-location
source_filename: amazon-pinpoint-endpoint-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-location-schema.json\",\n  \"title\": \"EndpointLocation\",\n  \"description\": \"Specifies geographic information about an endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"City\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the city where the endpoint is located.\"\n        }\n      ]\n    },\n    \"Country\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The two-character code, in ISO 3166-1 alpha-2 format, for the country or region where the endpoint is located. For example, US for the United States.\"\n        }\n      ]\n    },\n    \"Latitude\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"description\": \"The latitude coordinate of the endpoint location, rounded to one decimal place.\"\n        }\n      ]\n    },\n    \"Longitude\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"description\": \"The longitude coordinate of the endpoint location, rounded to one decimal place.\"\n        }\n      ]\n    },\n    \"PostalCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The postal or ZIP code for the area where the endpoint is located.\"\n        }\n      ]\n    },\n    \"Region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the region where the endpoint is located. For locations\
  \ in the United States, this value is the name of a state.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-location-schema.json
tags:
- AWS
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: EndpointLocation
---
