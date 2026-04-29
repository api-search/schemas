---
description: ''
layout: schema
name: tasking
properties_list:
- description: The contract id
  name: contractId
  type: object
- description: The order id
  name: orderId
  type: object
- description: The product type id
  name: productTypeId
  type: object
- description: The customer id
  name: customerId
  type: object
- description: The tasking id
  name: taskingId
  type: string
- description: The segment id
  name: segmentId
  type: object
- description: The licence id
  name: licenceId
  type: object
- description: The quotation id
  name: quotationId
  type: object
- description: ICR's list
  name: taskingIds
  type: array
- description: Number of items per page
  name: count
  type: integer
- description: Customer reference
  name: customerRef
  type: string
- description: Program name
  name: program
  type: string
- description: ICR Status
  name: status
  type: array
- description: mission name
  name: mission
  type: string
- description: Refer to one-tasking online documentation at http://www.intelligence-airbusds.com/ for more information
  name: progTypeNames
  type: string
- description: 'A date or date interval that must match the product acquisition date. Only taskings in this range are returned in the response. Example: [2017-01-01,2017-02-01[ to select all taskings done in January '
  name: acquisitionDate
  type: string
- description: 'A date or date interval that must match the icr end of period date. Only taskings in this range are returned in the response. Example: [2017-01-01,2017-02-01[ to select all taskings done in January 20'
  name: icrEndOfPeriodDate
  type: string
- description: Indicates whether the search should filter on proposed segments. If set to true, only ICR with proposed segments should be returned. If set to false, only ICR with no proposed segments. If not set, re
  name: hasProposedSegments
  type: boolean
- description: The desired page, starting from 1 for the first page.
  name: startPage
  type: integer
- description: 'A sorting request to the server conforming the OpenSearch SRU specification. Example: sortKeys=acquisitionDate,,0 meaning a request to sort by newest acquired image first or sortKeys=cloudCover,,1 to '
  name: sortKeys
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-tasking-schema.json
slug: oneatlas-tasking
source_filename: oneatlas-tasking-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-tasking-schema.json\",\n  \"title\": \"tasking\",\n  \"properties\": {\n    \"contractId\": {\n      \"name\": \"contractId\",\n      \"in\": \"path\",\n      \"required\": true,\n      \"description\": \"The contract id\",\n      \"schema\": {\n        \"type\": \"string\"\n      }\n    },\n    \"orderId\": {\n      \"name\": \"orderId\",\n      \"in\": \"path\",\n      \"required\": true,\n      \"description\": \"The order id\",\n      \"schema\": {\n        \"type\": \"string\"\n      }\n    },\n    \"productTypeId\": {\n      \"name\": \"productTypeId\",\n      \"in\": \"path\",\n      \"required\": true,\n      \"description\": \"The product type id\",\n      \"schema\": {\n        \"type\": \"string\"\n      }\n    },\n    \"customerId\": {\n      \"name\": \"customerId\",\n      \"in\"\
  : \"path\",\n      \"required\": true,\n      \"description\": \"The customer id\",\n      \"schema\": {\n        \"type\": \"string\"\n      }\n    },\n    \"taskingId\": {\n      \"name\": \"taskingId\",\n      \"in\": \"path\",\n      \"required\": true,\n      \"description\": \"The tasking id\",\n      \"type\": \"string\",\n      \"schema\": {\n        \"type\": \"string\"\n      }\n    },\n    \"segmentId\": {\n      \"name\": \"segmentId\",\n      \"in\": \"path\",\n      \"required\": true,\n      \"description\": \"The segment id\",\n      \"schema\": {\n        \"type\": \"string\"\n      }\n    },\n    \"licenceId\": {\n      \"name\": \"licenceId\",\n      \"in\": \"path\",\n      \"required\": true,\n      \"description\": \"The licence id\",\n      \"schema\": {\n        \"type\": \"string\"\n      }\n    },\n    \"quotationId\": {\n      \"name\": \"quotationId\",\n      \"in\": \"path\",\n      \"required\": true,\n      \"description\": \"The quotation id\",\n      \"\
  schema\": {\n        \"type\": \"string\"\n      }\n    },\n    \"taskingIds\": {\n      \"name\": \"taskingIds\",\n      \"in\": \"query\",\n      \"description\": \"ICR's list\",\n      \"type\": \"array\",\n      \"schema\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"count\": {\n      \"name\": \"count\",\n      \"in\": \"query\",\n      \"description\": \"Number of items per page\",\n      \"type\": \"integer\",\n      \"schema\": {\n        \"type\": \"integer\",\n        \"default\": 10\n      }\n    },\n    \"customerRef\": {\n      \"name\": \"customerRef\",\n      \"in\": \"query\",\n      \"description\": \"Customer reference\",\n      \"type\": \"string\",\n      \"schema\": {\n        \"type\": \"string\"\n      }\n    },\n    \"program\": {\n      \"name\": \"program\",\n      \"in\": \"query\",\n      \"description\": \"Program name\",\n      \"type\": \"string\",\n      \"schema\": {\n        \"\
  type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"name\": \"status\",\n      \"in\": \"query\",\n      \"description\": \"ICR Status\",\n      \"type\": \"array\",\n      \"schema\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Feasibility study in progress\",\n            \"In Progress\",\n            \"Paused\",\n            \"Canceled\",\n            \"Completed\"\n          ]\n        }\n      }\n    },\n    \"mission\": {\n      \"name\": \"mission\",\n      \"in\": \"query\",\n      \"description\": \"mission name\",\n      \"type\": \"string\",\n      \"schema\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"SPOT\",\n          \"PLEIADES\"\n        ]\n      }\n    },\n    \"progTypeNames\": {\n      \"name\": \"progTypeNames\",\n      \"in\": \"query\",\n      \"description\": \"Refer to one-tasking online documentation at http://www.intelligence-airbusds.com/ for more\
  \ information\",\n      \"type\": \"string\",\n      \"schema\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"ONEDAY\",\n          \"ONENOW\",\n          \"ONEPLAN\",\n          \"ONESERIES\"\n        ]\n      }\n    },\n    \"acquisitionDate\": {\n      \"name\": \"acquisitionDate\",\n      \"in\": \"query\",\n      \"description\": \"A date or date interval that must match the product acquisition date. Only taskings in this range are returned in the response. Example: [2017-01-01,2017-02-01[ to select all taskings done in January 2017.\",\n      \"type\": \"string\",\n      \"schema\": {\n        \"type\": \"string\",\n        \"format\": \"Interval of dates in ISO 8601\"\n      }\n    },\n    \"icrEndOfPeriodDate\": {\n      \"name\": \"icrEndOfPeriodDate\",\n      \"in\": \"query\",\n      \"description\": \"A date or date interval that must match the icr end of period date. Only taskings in this range are returned in the response. Example: [2017-01-01,2017-02-01[\
  \ to select all taskings done in January 2017.\",\n      \"type\": \"string\",\n      \"schema\": {\n        \"type\": \"string\",\n        \"format\": \"Interval of dates in ISO 8601\"\n      }\n    },\n    \"hasProposedSegments\": {\n      \"name\": \"hasProposedSegments\",\n      \"in\": \"query\",\n      \"description\": \"Indicates whether the search should filter on proposed segments. If set to true, only ICR with proposed segments should be returned. If set to false, only ICR with no proposed segments. If not set, returns all ICR ignoring presence/absence of proposed segments\",\n      \"type\": \"boolean\",\n      \"schema\": {\n        \"type\": \"boolean\"\n      }\n    },\n    \"startPage\": {\n      \"name\": \"startPage\",\n      \"in\": \"query\",\n      \"description\": \"The desired page, starting from 1 for the first page.\",\n      \"type\": \"integer\",\n      \"schema\": {\n        \"type\": \"integer\",\n        \"default\": 1\n      }\n    },\n    \"sortKeys\": {\n\
  \      \"name\": \"sortKeys\",\n      \"in\": \"query\",\n      \"description\": \"A sorting request to the server conforming the OpenSearch SRU specification. Example: sortKeys=acquisitionDate,,0 meaning a request to sort by newest acquired image first or sortKeys=cloudCover,,1 to sort by the smallest cloud coverage percentage. Available values are: status, startDate, endDate, taskingProgress\",\n      \"type\": \"string\",\n      \"schema\": {\n        \"type\": \"string\",\n        \"format\": \"OpenSearch SRU\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-tasking-schema.json
tags:
- Imagery
- Satellites
title: tasking
---
