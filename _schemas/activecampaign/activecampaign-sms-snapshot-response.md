---
description: SnapshotResponse schema from ActiveCampaign API
layout: schema
name: SnapshotResponse
properties_list:
- description: ''
  name: snapshot
  type: object
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-snapshot-response-schema.json
slug: activecampaign-sms-snapshot-response
source_filename: activecampaign-sms-snapshot-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-snapshot-response-schema.json\",\n  \"title\": \"SnapshotResponse\",\n  \"description\": \"SnapshotResponse schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"snapshot\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"campaigns\": {\n          \"type\": \"integer\"\n        },\n        \"sends\": {\n          \"type\": \"integer\"\n        },\n        \"deliveries\": {\n          \"type\": \"integer\"\n        },\n        \"clicks\": {\n          \"type\": \"integer\"\n        },\n        \"replies\": {\n          \"type\": \"integer\"\n        },\n        \"failures\": {\n          \"type\": \"integer\"\n        },\n        \"optOuts\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-snapshot-response-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: SnapshotResponse
---
