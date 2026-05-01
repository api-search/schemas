---
description: UpdateJobShipmentStateRequest schema from Amazon Snow Family API
layout: schema
name: UpdateJobShipmentStateRequest
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: ShipmentState
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-update-job-shipment-state-request-schema.json
slug: amazon-snow-family-update-job-shipment-state-request
source_filename: amazon-snow-family-update-job-shipment-state-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-update-job-shipment-state-request-schema.json\",\n  \"title\": \"UpdateJobShipmentStateRequest\",\n  \"description\": \"UpdateJobShipmentStateRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The job ID of the job whose shipment date you want to update, for example <code>JID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    },\n    \"ShipmentState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShipmentState\"\n        },\n        {\n          \"description\": \"<p>The state of a device when it is being shipped. </p> <p>Set to <code>RECEIVED</code>\
  \ when the device arrives at your location.</p> <p>Set to <code>RETURNED</code> when you have returned the device to Amazon Web Services.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobId\",\n    \"ShipmentState\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-update-job-shipment-state-request-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: UpdateJobShipmentStateRequest
---
