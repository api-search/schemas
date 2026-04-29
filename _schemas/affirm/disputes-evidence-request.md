---
description: Request body for submitting evidence to contest a dispute. May include file references, textual explanations, and shipping/tracking details.
layout: schema
name: EvidenceRequest
properties_list:
- description: Array of file identifiers uploaded via the Files API to attach as documentary evidence.
  name: files
  type: array
- description: Textual explanation of the merchant's position and why the dispute should be decided in the merchant's favor.
  name: explanation
  type: string
- description: Shipment tracking number demonstrating that the order was delivered as expected.
  name: tracking_number
  type: string
- description: Name of the shipping carrier used for the disputed order.
  name: shipping_carrier
  type: string
- description: Description or summary of communications with the customer regarding the disputed order.
  name: customer_communication
  type: string
- description: Description of the merchant's refund policy as shown to the customer at the time of purchase.
  name: refund_policy_disclosure
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/disputes-evidence-request-schema.json
slug: disputes-evidence-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/disputes-evidence-request-schema.json\",\n  \"title\": \"EvidenceRequest\",\n  \"description\": \"Request body for submitting evidence to contest a dispute. May include file references, textual explanations, and shipping/tracking details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"Array of file identifiers uploaded via the Files API to attach as documentary evidence.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"explanation\": {\n      \"type\": \"string\",\n      \"description\": \"Textual explanation of the merchant's position and why the dispute should be decided in the merchant's favor.\",\n      \"example\": \"example_value\"\n    },\n    \"\
  tracking_number\": {\n      \"type\": \"string\",\n      \"description\": \"Shipment tracking number demonstrating that the order was delivered as expected.\",\n      \"example\": \"example_value\"\n    },\n    \"shipping_carrier\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the shipping carrier used for the disputed order.\",\n      \"example\": \"example_value\"\n    },\n    \"customer_communication\": {\n      \"type\": \"string\",\n      \"description\": \"Description or summary of communications with the customer regarding the disputed order.\",\n      \"example\": \"example_value\"\n    },\n    \"refund_policy_disclosure\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the merchant's refund policy as shown to the customer at the time of purchase.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/disputes-evidence-request-schema.json
tags: []
title: EvidenceRequest
---
