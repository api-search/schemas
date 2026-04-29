---
description: Provides information about all the export jobs that are associated with an application or segment. An export job is a job that exports endpoint definitions to a file.
layout: schema
name: ExportJobsResponse
properties_list:
- description: ''
  name: Item
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-export-jobs-response-schema.json
slug: amazon-pinpoint-export-jobs-response
source_filename: amazon-pinpoint-export-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-export-jobs-response-schema.json\",\n  \"title\": \"ExportJobsResponse\",\n  \"description\": \"Provides information about all the export jobs that are associated with an application or segment. An export job is a job that exports endpoint definitions to a file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Item\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfExportJobResponse\"\n        },\n        {\n          \"description\": \"An array of responses, one for each export job that's associated with the application (Export Jobs resource) or segment (Segment Export Jobs resource).\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n\
  \          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null if there are no additional pages.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Item\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-export-jobs-response-schema.json
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
title: ExportJobsResponse
---
