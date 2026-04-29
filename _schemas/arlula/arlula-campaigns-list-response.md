---
description: Paginated list of campaigns.
layout: schema
name: CampaignsListResponse
properties_list:
- description: ''
  name: campaigns
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-campaigns-list-response-schema.json
slug: arlula-campaigns-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/campaigns-list-response.json\",\n  \"title\": \"CampaignsListResponse\",\n  \"description\": \"Paginated list of campaigns.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaigns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"https://arlula.com/json-schema/campaign.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-campaigns-list-response-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: CampaignsListResponse
---
