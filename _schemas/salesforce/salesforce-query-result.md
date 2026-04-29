---
description: The result of a Salesforce SOQL (Salesforce Object Query Language) query executed via the REST API /query or /queryAll endpoints. Contains the total number of matching records, a pagination flag, an optional URL for the next page of results, and an array of SObject records matching the query.
layout: schema
name: Salesforce SOQL Query Result
properties_list:
- description: 'The total number of records matching the SOQL query across all pages. This is the count of all matching records, not just the records in the current page. May be larger than the length of the records '
  name: totalSize
  type: integer
- description: Whether all query results have been retrieved and included in the current response. If true, the records array contains all matching records. If false, additional pages of results are available via th
  name: done
  type: boolean
- description: The relative URL to retrieve the next page of query results. Only present when done is false, indicating there are more records beyond the current page. Pass this URL to the GET /query/{queryId} endpo
  name: nextRecordsUrl
  type: string
- description: An array of Salesforce SObject records matching the SOQL query. Each record is an object with an attributes property (containing type and url) plus field name/value pairs for all fields included in th
  name: records
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-query-result-schema.json
slug: salesforce-query-result
source_filename: salesforce-query-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-query-result-schema.json\",\n  \"title\": \"Salesforce SOQL Query Result\",\n  \"description\": \"The result of a Salesforce SOQL (Salesforce Object Query Language) query executed via the REST API /query or /queryAll endpoints. Contains the total number of matching records, a pagination flag, an optional URL for the next page of results, and an array of SObject records matching the query.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"totalSize\",\n    \"done\",\n    \"records\"\n  ],\n  \"properties\": {\n    \"totalSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of records matching the SOQL query across all pages. This is the count of all matching records, not just the records in the current page. May be larger than the length of the records array when\
  \ results are paginated.\",\n      \"minimum\": 0\n    },\n    \"done\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether all query results have been retrieved and included in the current response. If true, the records array contains all matching records. If false, additional pages of results are available via the nextRecordsUrl.\"\n    },\n    \"nextRecordsUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The relative URL to retrieve the next page of query results. Only present when done is false, indicating there are more records beyond the current page. Pass this URL to the GET /query/{queryId} endpoint to retrieve subsequent pages. Continues paginating until done is true.\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"An array of Salesforce SObject records matching the SOQL query. Each record is an object with an attributes property (containing type and url) plus field name/value pairs for\
  \ all fields included in the SELECT clause. May be an empty array if no records match the query.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single Salesforce SObject record returned by the query. Contains an attributes object with record type metadata, plus field values for all fields requested in the SOQL SELECT clause.\",\n        \"required\": [\n          \"attributes\"\n        ],\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"object\",\n            \"description\": \"Metadata attributes for this SObject record, identifying its type and REST API URL.\",\n            \"required\": [\n              \"type\"\n            ],\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"The API name of the Salesforce SObject type (e.g., Account, Contact, Opportunity). Identifies what kind of record this is.\"\n              },\n             \
  \ \"url\": {\n                \"type\": \"string\",\n                \"format\": \"uri\",\n                \"description\": \"The relative REST API URL for this specific record. Use this URL to retrieve, update, or delete the record.\"\n              }\n            },\n            \"additionalProperties\": false\n          }\n        },\n        \"additionalProperties\": true\n      }\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-query-result-schema.json
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
title: Salesforce SOQL Query Result
---
