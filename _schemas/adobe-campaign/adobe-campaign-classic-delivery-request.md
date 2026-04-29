---
description: SOAP envelope containing the delivery internal name or ID for preparation and sending operations.
layout: schema
name: DeliveryRequest
properties_list:
- description: Internal ID of the delivery.
  name: deliveryId
  type: integer
- description: Internal name of the delivery.
  name: deliveryName
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-delivery-request-schema.json
slug: adobe-campaign-classic-delivery-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-delivery-request-schema.json\",\n  \"title\": \"DeliveryRequest\",\n  \"description\": \"SOAP envelope containing the delivery internal name or ID for preparation and sending operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deliveryId\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal ID of the delivery.\",\n      \"example\": 42\n    },\n    \"deliveryName\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name of the delivery.\",\n      \"example\": \"Example Campaign\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-delivery-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: DeliveryRequest
---
