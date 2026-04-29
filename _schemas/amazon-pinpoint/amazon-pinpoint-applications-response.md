---
description: Provides information about all of your applications.
layout: schema
name: ApplicationsResponse
properties_list:
- description: ''
  name: Item
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-applications-response-schema.json
slug: amazon-pinpoint-applications-response
source_filename: amazon-pinpoint-applications-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-applications-response-schema.json\",\n  \"title\": \"ApplicationsResponse\",\n  \"description\": \"Provides information about all of your applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Item\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfApplicationResponse\"\n        },\n        {\n          \"description\": \"An array of responses, one for each application that was returned.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null if there are no additional pages.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-applications-response-schema.json
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
title: ApplicationsResponse
---
