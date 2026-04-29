---
description: Information about a line item shipment.
layout: schema
name: ShipmentInformation
properties_list:
- description: ''
  name: ShipmentTrackingNumber
  type: object
- description: ''
  name: ShipmentCarrier
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-shipment-information-schema.json
slug: openapi-shipment-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-shipment-information-schema.json\",\n  \"title\": \"ShipmentInformation\",\n  \"description\": \" Information about a line item shipment. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ShipmentTrackingNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrackingId\"\n        },\n        {\n          \"description\": \" The tracking number of the shipment. \"\n        }\n      ]\n    },\n    \"ShipmentCarrier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShipmentCarrier\"\n        },\n        {\n          \"description\": \" The carrier of the shipment. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-shipment-information-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: ShipmentInformation
---
