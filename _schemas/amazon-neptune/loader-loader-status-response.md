---
description: LoaderStatusResponse schema from Neptune
layout: schema
name: LoaderStatusResponse
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: payload
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/loader-loader-status-response-schema.json
slug: loader-loader-status-response
source_filename: loader-loader-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/loader-loader-status-response-schema.json\",\n  \"title\": \"LoaderStatusResponse\",\n  \"description\": \"LoaderStatusResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"feedCount\": {\n          \"type\": \"array\",\n          \"description\": \"Count of feeds processed.\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        },\n        \"overallStatus\": {\n          \"type\": \"object\",\n          \"description\": \"Overall status of the load job.\",\n          \"properties\": {\n            \"fullUri\": {\n              \"type\": \"string\",\n              \"description\": \"The S3 URI of the data source.\"\
  \n            },\n            \"runNumber\": {\n              \"type\": \"integer\",\n              \"description\": \"The run number for this load.\"\n            },\n            \"retryNumber\": {\n              \"type\": \"integer\",\n              \"description\": \"The retry number.\"\n            },\n            \"status\": {\n              \"type\": \"string\",\n              \"description\": \"The job status (LOAD_NOT_STARTED, LOAD_IN_PROGRESS, LOAD_COMPLETED, LOAD_CANCELLED_BY_USER, LOAD_CANCELLED_DUE_TO_ERRORS, LOAD_FAILED, LOAD_UNEXPECTED_ERROR, LOAD_DATA_DEADLOCK, LOAD_DATA_FAILED_DUE_TO_FEED_MODIFIED_OR_DELETED, LOAD_S3_READ_ERROR, LOAD_S3_ACCESS_DENIED_ERROR, LOAD_COMMITTED_W_WRITE_CONFLICTS).\",\n              \"enum\": [\n                \"LOAD_NOT_STARTED\",\n                \"LOAD_IN_PROGRESS\",\n                \"LOAD_COMPLETED\",\n                \"LOAD_CANCELLED_BY_USER\",\n                \"LOAD_CANCELLED_DUE_TO_ERRORS\",\n                \"LOAD_FAILED\",\n      \
  \          \"LOAD_UNEXPECTED_ERROR\",\n                \"LOAD_DATA_DEADLOCK\",\n                \"LOAD_DATA_FAILED_DUE_TO_FEED_MODIFIED_OR_DELETED\",\n                \"LOAD_S3_READ_ERROR\",\n                \"LOAD_S3_ACCESS_DENIED_ERROR\",\n                \"LOAD_COMMITTED_W_WRITE_CONFLICTS\"\n              ]\n            },\n            \"totalTimeSpent\": {\n              \"type\": \"integer\",\n              \"description\": \"Total time spent on the load in seconds.\"\n            },\n            \"startTime\": {\n              \"type\": \"integer\",\n              \"description\": \"Start time as a Unix timestamp.\"\n            },\n            \"totalRecords\": {\n              \"type\": \"integer\",\n              \"description\": \"Total records processed.\"\n            },\n            \"totalDuplicates\": {\n              \"type\": \"integer\",\n              \"description\": \"Total duplicate records encountered.\"\n            },\n            \"parsingErrors\": {\n       \
  \       \"type\": \"integer\",\n              \"description\": \"Total parsing errors.\"\n            },\n            \"datatypeMismatchErrors\": {\n              \"type\": \"integer\",\n              \"description\": \"Total datatype mismatch errors.\"\n            },\n            \"insertErrors\": {\n              \"type\": \"integer\",\n              \"description\": \"Total insert errors.\"\n            }\n          }\n        },\n        \"failedFeeds\": {\n          \"type\": \"array\",\n          \"description\": \"Details about failed feeds.\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        },\n        \"errors\": {\n          \"type\": \"object\",\n          \"description\": \"Error details (when errors=true was requested).\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/loader-loader-status-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: LoaderStatusResponse
---
