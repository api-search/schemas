---
description: Provides a single value and metadata about that value as part of an array of query results for a standard metric that applies to an application, campaign, or journey.
layout: schema
name: ResultRowValue
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-result-row-value-schema.json
slug: amazon-pinpoint-result-row-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-result-row-value-schema.json\",\n  \"title\": \"ResultRowValue\",\n  \"description\": \"Provides a single value and metadata about that value as part of an array of query results for a standard metric that applies to an application, campaign, or journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The friendly name of the metric whose value is specified by the Value property.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The data type of the value specified by the Value property.\"\n        }\n\
  \      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"In a Values object, the value for the metric that the query retrieved data for. In a GroupedBys object, the value for the field that was used to group data in a result set that contains multiple results (Values objects).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Type\",\n    \"Value\",\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-result-row-value-schema.json
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
title: ResultRowValue
---
