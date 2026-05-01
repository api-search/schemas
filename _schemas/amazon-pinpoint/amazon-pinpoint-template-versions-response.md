---
description: Provides information about all the versions of a specific message template.
layout: schema
name: TemplateVersionsResponse
properties_list:
- description: ''
  name: Item
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: RequestID
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-template-versions-response-schema.json
slug: amazon-pinpoint-template-versions-response
source_filename: amazon-pinpoint-template-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-template-versions-response-schema.json\",\n  \"title\": \"TemplateVersionsResponse\",\n  \"description\": \"Provides information about all the versions of a specific message template.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Item\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfTemplateVersionResponse\"\n        },\n        {\n          \"description\": \"An array of responses, one for each version of the message template.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The message that's returned from the API for the request to retrieve information about all the versions of the message template.\"\
  \n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null if there are no additional pages.\"\n        }\n      ]\n    },\n    \"RequestID\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the request to retrieve information about all the versions of the message template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Item\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-template-versions-response-schema.json
tags:
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
title: TemplateVersionsResponse
---
