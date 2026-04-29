---
description: Provides the results of a query that retrieved the data for a standard metric that applies to an application, campaign, or journey.
layout: schema
name: BaseKpiResult
properties_list:
- description: ''
  name: Rows
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-base-kpi-result-schema.json
slug: amazon-pinpoint-base-kpi-result
source_filename: amazon-pinpoint-base-kpi-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-base-kpi-result-schema.json\",\n  \"title\": \"BaseKpiResult\",\n  \"description\": \"Provides the results of a query that retrieved the data for a standard metric that applies to an application, campaign, or journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfResultRow\"\n        },\n        {\n          \"description\": \"An array of objects that provides the results of a query that retrieved the data for a standard metric that applies to an application, campaign, or journey.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Rows\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-base-kpi-result-schema.json
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
title: BaseKpiResult
---
