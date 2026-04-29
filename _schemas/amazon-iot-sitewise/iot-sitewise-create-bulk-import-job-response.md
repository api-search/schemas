---
description: CreateBulkImportJobResponse schema
layout: schema
name: CreateBulkImportJobResponse
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: jobName
  type: object
- description: ''
  name: jobStatus
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-create-bulk-import-job-response-schema.json
slug: iot-sitewise-create-bulk-import-job-response
source_filename: iot-sitewise-create-bulk-import-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-bulk-import-job-response-schema.json\",\n  \"title\": \"CreateBulkImportJobResponse\",\n  \"description\": \"CreateBulkImportJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the job.\"\n        }\n      ]\n    },\n    \"jobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The unique name that helps identify the job request.\"\n        }\n      ]\n    },\n    \"jobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\"\
  : \"<p>The status of the bulk import job can be one of following values.</p> <ul> <li> <p> <code>PENDING</code> \\u2013 IoT SiteWise is waiting for the current bulk import job to finish.</p> </li> <li> <p> <code>CANCELLED</code> \\u2013 The bulk import job has been canceled.</p> </li> <li> <p> <code>RUNNING</code> \\u2013 IoT SiteWise is processing your request to import your data from Amazon S3.</p> </li> <li> <p> <code>COMPLETED</code> \\u2013 IoT SiteWise successfully completed your request to import data from Amazon S3.</p> </li> <li> <p> <code>FAILED</code> \\u2013 IoT SiteWise couldn't process your request to import data from Amazon S3. You can use logs saved in the specified error report location in Amazon S3 to troubleshoot issues.</p> </li> <li> <p> <code>COMPLETED_WITH_FAILURES</code> \\u2013 IoT SiteWise completed your request to import data from Amazon S3 with errors. You can use logs saved in the specified error report location in Amazon S3 to troubleshoot issues.</p> </li>\
  \ </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\",\n    \"jobName\",\n    \"jobStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-bulk-import-job-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: CreateBulkImportJobResponse
---
