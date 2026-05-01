---
description: The <code>Status</code> and <code>TrackingNumber</code> information for an inbound or outbound shipment.
layout: schema
name: Shipment
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: TrackingNumber
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-shipment-schema.json
slug: amazon-snow-family-shipment
source_filename: amazon-snow-family-shipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-shipment-schema.json\",\n  \"title\": \"Shipment\",\n  \"description\": \"The <code>Status</code> and <code>TrackingNumber</code> information for an inbound or outbound shipment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Status information for a shipment.\"\n        }\n      ]\n    },\n    \"TrackingNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The tracking number for this job. Using this tracking number with your region's carrier's website, you can track a Snow device as the carrier transports it.</p> <p>For India,\
  \ the carrier is Amazon Logistics. For all other regions, UPS is the carrier.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-shipment-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: Shipment
---
