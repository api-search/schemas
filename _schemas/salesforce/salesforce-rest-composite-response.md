---
description: The result of a composite request, containing results for each subrequest in order.
layout: schema
name: CompositeResponse
properties_list:
- description: Array of results corresponding to each subrequest, in the same order as the input compositeRequest array.
  name: compositeResponse
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-rest-composite-response-schema.json
slug: salesforce-rest-composite-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result of a composite request, containing results for each subrequest in order.\\n\",\n  \"properties\": {\n    \"compositeResponse\": {\n      \"type\": \"array\",\n      \"description\": \"Array of results corresponding to each subrequest, in the same order as the input compositeRequest array.\\n\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"body\": {\n            \"type\": \"object\",\n            \"description\": \"Response body of the subrequest.\"\n          },\n          \"httpHeaders\": {\n            \"type\": \"object\",\n            \"description\": \"Response HTTP headers for the subrequest.\"\n          },\n          \"httpStatusCode\": {\n            \"type\": \"integer\",\n            \"description\": \"HTTP status code of the subrequest.\"\n          },\n          \"referenceId\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"The reference ID of the corresponding subrequest.\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompositeResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-rest-composite-response-schema.json
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
title: CompositeResponse
---
