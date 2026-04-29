---
description: SingleCampaignRequest schema from AB Tasty Decision API
layout: schema
name: SingleCampaignRequest
properties_list: []
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-single-campaign-request-schema.json
slug: decision-api-single-campaign-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-single-campaign-request-schema.json\",\n  \"title\": \"SingleCampaignRequest\",\n  \"description\": \"SingleCampaignRequest schema from AB Tasty Decision API\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/CampaignRequest\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"format_response\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, response will be formatted according to modification type\",\n          \"default\": false\n        },\n        \"default_redirect_url\": {\n          \"type\": \"string\",\n          \"description\": \"Default URL for 302 redirect if no modification redirection is defined\",\n          \"example\": \"https://example.com/default\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-single-campaign-request-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: SingleCampaignRequest
---
