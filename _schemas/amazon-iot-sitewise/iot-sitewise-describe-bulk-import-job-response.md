---
description: DescribeBulkImportJobResponse schema
layout: schema
name: DescribeBulkImportJobResponse
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
- description: ''
  name: jobRoleArn
  type: object
- description: ''
  name: files
  type: object
- description: ''
  name: errorReportLocation
  type: object
- description: ''
  name: jobConfiguration
  type: object
- description: ''
  name: jobCreationDate
  type: object
- description: ''
  name: jobLastUpdateDate
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-bulk-import-job-response-schema.json
slug: iot-sitewise-describe-bulk-import-job-response
source_filename: iot-sitewise-describe-bulk-import-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-bulk-import-job-response-schema.json\",\n  \"title\": \"DescribeBulkImportJobResponse\",\n  \"description\": \"DescribeBulkImportJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the job.\"\n        }\n      ]\n    },\n    \"jobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The unique name that helps identify the job request.\"\n        }\n      ]\n    },\n    \"jobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\"\
  : \"<p>The status of the bulk import job can be one of following values.</p> <ul> <li> <p> <code>PENDING</code> \\u2013 IoT SiteWise is waiting for the current bulk import job to finish.</p> </li> <li> <p> <code>CANCELLED</code> \\u2013 The bulk import job has been canceled.</p> </li> <li> <p> <code>RUNNING</code> \\u2013 IoT SiteWise is processing your request to import your data from Amazon S3.</p> </li> <li> <p> <code>COMPLETED</code> \\u2013 IoT SiteWise successfully completed your request to import data from Amazon S3.</p> </li> <li> <p> <code>FAILED</code> \\u2013 IoT SiteWise couldn't process your request to import data from Amazon S3. You can use logs saved in the specified error report location in Amazon S3 to troubleshoot issues.</p> </li> <li> <p> <code>COMPLETED_WITH_FAILURES</code> \\u2013 IoT SiteWise completed your request to import data from Amazon S3 with errors. You can use logs saved in the specified error report location in Amazon S3 to troubleshoot issues.</p> </li>\
  \ </ul>\"\n        }\n      ]\n    },\n    \"jobRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the IAM role that allows IoT SiteWise to read Amazon S3 data.\"\n        }\n      ]\n    },\n    \"files\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Files\"\n        },\n        {\n          \"description\": \"The files in the specified Amazon S3 bucket that contain your data.\"\n        }\n      ]\n    },\n    \"errorReportLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorReportLocation\"\n        },\n        {\n          \"description\": \"The Amazon S3 destination where errors associated with the job creation request are saved.\"\n        }\n      ]\n    },\n    \"jobConfiguration\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/JobConfiguration\"\n        },\n        {\n          \"description\": \"Contains the configuration information of a job, such as the file format used to save data in Amazon S3.\"\n        }\n      ]\n    },\n    \"jobCreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the job was created, in Unix epoch TIME.\"\n        }\n      ]\n    },\n    \"jobLastUpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the job was last updated, in Unix epoch time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\",\n    \"jobName\",\n    \"jobStatus\",\n    \"jobRoleArn\",\n    \"files\",\n    \"errorReportLocation\",\n    \"jobConfiguration\",\n    \"jobCreationDate\",\n    \"jobLastUpdateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-bulk-import-job-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribeBulkImportJobResponse
---
