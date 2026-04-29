---
description: A composite request containing an ordered series of subrequests where later requests can reference the results of earlier ones using reference IDs.
layout: schema
name: CompositeRequest
properties_list:
- description: If true, all subrequests must succeed or all changes are rolled back. If false, subrequests are processed independently.
  name: allOrNone
  type: boolean
- description: If true, similar subrequests are grouped for more efficient processing.
  name: collateSubrequests
  type: boolean
- description: Ordered array of subrequests. Later subrequests can reference results from earlier ones using @{referenceId.field} syntax.
  name: compositeRequest
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-rest-composite-request-schema.json
slug: salesforce-rest-composite-request
source_filename: salesforce-rest-composite-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A composite request containing an ordered series of subrequests where later requests can reference the results of earlier ones using reference IDs.\\n\",\n  \"properties\": {\n    \"allOrNone\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, all subrequests must succeed or all changes are rolled back. If false, subrequests are processed independently.\\n\",\n      \"example\": true\n    },\n    \"collateSubrequests\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, similar subrequests are grouped for more efficient processing.\\n\",\n      \"example\": true\n    },\n    \"compositeRequest\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered array of subrequests. Later subrequests can reference results from earlier ones using @{referenceId.field} syntax.\\n\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"\
  method\": {\n            \"type\": \"string\",\n            \"description\": \"HTTP method for this subrequest.\",\n            \"enum\": [\n              \"GET\",\n              \"POST\",\n              \"PATCH\",\n              \"DELETE\"\n            ]\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"description\": \"Relative URL for this subrequest.\"\n          },\n          \"referenceId\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for this subrequest. Used to reference this subrequest's results in subsequent subrequests.\\n\"\n          },\n          \"body\": {\n            \"type\": \"object\",\n            \"description\": \"Request body for POST and PATCH subrequests.\"\n          }\n        },\n        \"required\": [\n          \"method\",\n          \"url\",\n          \"referenceId\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"compositeRequest\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"CompositeRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-rest-composite-request-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: CompositeRequest
---
