---
description: Provides information about the status and settings of all the import jobs that are associated with an application or segment. An import job is a job that imports endpoint definitions from one or more files.
layout: schema
name: ImportJobsResponse
properties_list:
- description: ''
  name: Item
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-import-jobs-response-schema.json
slug: amazon-pinpoint-import-jobs-response
source_filename: amazon-pinpoint-import-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-import-jobs-response-schema.json\",\n  \"title\": \"ImportJobsResponse\",\n  \"description\": \"Provides information about the status and settings of all the import jobs that are associated with an application or segment. An import job is a job that imports endpoint definitions from one or more files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Item\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfImportJobResponse\"\n        },\n        {\n          \"description\": \"An array of responses, one for each import job that's associated with the application (Import Jobs resource) or segment (Segment Import Jobs resource).\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null if there are no additional pages.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Item\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-import-jobs-response-schema.json
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
title: ImportJobsResponse
---
