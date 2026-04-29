---
description: A capture campaign within an order.
layout: schema
name: Campaign
properties_list:
- description: Campaign identifier.
  name: campaignId
  type: string
- description: Parent order identifier.
  name: orderId
  type: string
- description: Campaign status.
  name: status
  type: string
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-campaign-schema.json
slug: arlula-campaign
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/campaign.json\",\n  \"title\": \"Campaign\",\n  \"description\": \"A capture campaign within an order.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignId\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign identifier.\",\n      \"examples\": [\n        \"campaign-001\"\n      ]\n    },\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent order identifier.\",\n      \"examples\": [\n        \"order-a1b2c3d4\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign status.\",\n      \"examples\": [\n        \"completed\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-campaign-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: Campaign
---
