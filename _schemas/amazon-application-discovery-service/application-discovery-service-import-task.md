---
description: ImportTask schema from Amazon Application Discovery Service API
layout: schema
name: ImportTask
properties_list:
- description: The unique ID for a specific import task.
  name: importTaskId
  type: string
- description: A unique token used to prevent the same import request from occurring more than once.
  name: clientRequestToken
  type: string
- description: A descriptive name for an import task.
  name: name
  type: string
- description: The URL for your import file that you've uploaded to Amazon S3.
  name: importUrl
  type: string
- description: The status of the import task.
  name: status
  type: string
- description: The time that the import task request was made, presented in the Unix time stamp format.
  name: importRequestTime
  type: string
- description: The time that the import task request finished, presented in the Unix time stamp format.
  name: importCompletionTime
  type: string
- description: The time that the import task request was deleted, presented in the Unix time stamp format.
  name: importDeletedTime
  type: string
- description: The total number of server records in the import file that were successfully imported.
  name: serverImportSuccess
  type: integer
- description: The total number of server records in the import file that failed to be imported.
  name: serverImportFailure
  type: integer
- description: The total number of application records in the import file that were successfully imported.
  name: applicationImportSuccess
  type: integer
- description: The total number of application records in the import file that failed to be imported.
  name: applicationImportFailure
  type: integer
- description: A link to a compressed archive folder (in the ZIP format) of all errors and failed entries that were detected, organized according to the type of error.
  name: errorsAndFailedEntriesZip
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-import-task-schema.json
slug: application-discovery-service-import-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-import-task-schema.json\",\n  \"title\": \"ImportTask\",\n  \"description\": \"ImportTask schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"importTaskId\": {\n      \"type\": \"string\",\n      \"example\": \"import-task-500123\",\n      \"description\": \"The unique ID for a specific import task.\"\n    },\n    \"clientRequestToken\": {\n      \"type\": \"string\",\n      \"example\": \"client-token-500123\",\n      \"description\": \"A unique token used to prevent the same import request from occurring more than once.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Server Inventory Import April 2026\",\n      \"description\": \"A descriptive name for an import task.\"\
  \n    },\n    \"importUrl\": {\n      \"type\": \"string\",\n      \"example\": \"s3://my-bucket/server-inventory.csv\",\n      \"description\": \"The URL for your import file that you've uploaded to Amazon S3.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IMPORT_IN_PROGRESS\",\n        \"IMPORT_COMPLETE\",\n        \"IMPORT_COMPLETE_WITH_ERRORS\",\n        \"IMPORT_FAILED\",\n        \"IMPORT_FAILED_SERVER_LIMIT_EXCEEDED\",\n        \"IMPORT_FAILED_RECORD_LIMIT_EXCEEDED\",\n        \"DELETE_IN_PROGRESS\",\n        \"DELETE_COMPLETE\",\n        \"DELETE_FAILED\",\n        \"DELETE_FAILED_LIMIT_EXCEEDED\",\n        \"INTERNAL_ERROR\"\n      ],\n      \"example\": \"IMPORT_COMPLETE\",\n      \"description\": \"The status of the import task.\"\n    },\n    \"importRequestTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-19T10:00:00Z\",\n      \"description\": \"The time that the import task request was made, presented in the Unix\
  \ time stamp format.\"\n    },\n    \"importCompletionTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-19T10:05:00Z\",\n      \"description\": \"The time that the import task request finished, presented in the Unix time stamp format.\"\n    },\n    \"importDeletedTime\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The time that the import task request was deleted, presented in the Unix time stamp format.\"\n    },\n    \"serverImportSuccess\": {\n      \"type\": \"integer\",\n      \"example\": 42,\n      \"description\": \"The total number of server records in the import file that were successfully imported.\"\n    },\n    \"serverImportFailure\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"The total number of server records in the import file that failed to be imported.\"\n    },\n    \"applicationImportSuccess\": {\n      \"type\": \"integer\",\n      \"example\": 5,\n      \"description\"\
  : \"The total number of application records in the import file that were successfully imported.\"\n    },\n    \"applicationImportFailure\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"The total number of application records in the import file that failed to be imported.\"\n    },\n    \"errorsAndFailedEntriesZip\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"A link to a compressed archive folder (in the ZIP format) of all errors and failed entries that were detected, organized according to the type of error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-import-task-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: ImportTask
---
