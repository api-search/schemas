---
description: Provides the results of a query that retrieved the data for a standard metric that applies to an application, campaign, or journey.
layout: schema
name: ResultRow
properties_list:
- description: ''
  name: GroupedBys
  type: object
- description: ''
  name: Values
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-result-row-schema.json
slug: amazon-pinpoint-result-row
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-result-row-schema.json\",\n  \"title\": \"ResultRow\",\n  \"description\": \"Provides the results of a query that retrieved the data for a standard metric that applies to an application, campaign, or journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupedBys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfResultRowValue\"\n        },\n        {\n          \"description\": \"An array of objects that defines the field and field values that were used to group data in a result set that contains multiple results. This value is null if the data in a result set isn\\u2019t grouped.\"\n        }\n      ]\n    },\n    \"Values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfResultRowValue\"\n        },\n\
  \        {\n          \"description\": \"An array of objects that provides pre-aggregated values for a standard metric that applies to an application, campaign, or journey.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GroupedBys\",\n    \"Values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-result-row-schema.json
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
title: ResultRow
---
