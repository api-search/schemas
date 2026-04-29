---
description: Continuous Web Job Information.
layout: schema
name: ContinuousWebJob
properties_list:
- description: ContinuousWebJob resource specific properties
  name: properties
  type: object
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-continuous-web-job-schema.json
slug: azure-functions-continuous-web-job
source_filename: azure-functions-continuous-web-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-continuous-web-job-schema.json\",\n  \"title\": \"ContinuousWebJob\",\n  \"description\": \"Continuous Web Job Information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"description\": \"ContinuousWebJob resource specific properties\",\n      \"properties\": {\n        \"detailed_status\": {\n          \"description\": \"Detailed status.\",\n          \"type\": \"string\"\n        },\n        \"error\": {\n          \"description\": \"Error information.\",\n          \"type\": \"string\"\n        },\n        \"extra_info_url\": {\n          \"description\": \"Extra Info URL.\",\n          \"type\": \"string\"\n        },\n        \"log_url\": {\n          \"description\": \"Log URL.\",\n          \"type\": \"string\"\n        },\n        \"run_command\"\
  : {\n          \"description\": \"Run command.\",\n          \"type\": \"string\"\n        },\n        \"settings\": {\n          \"additionalProperties\": {\n            \"type\": \"object\"\n          },\n          \"description\": \"Job settings.\",\n          \"type\": \"object\"\n        },\n        \"status\": {\n          \"description\": \"Job status.\",\n          \"enum\": [\n            \"Initializing\",\n            \"Starting\",\n            \"Running\",\n            \"PendingRestart\",\n            \"Stopped\"\n          ],\n          \"type\": \"string\",\n          \"x-ms-enum\": {\n            \"modelAsString\": false,\n            \"name\": \"ContinuousWebJobStatus\"\n          }\n        },\n        \"url\": {\n          \"description\": \"Job URL.\",\n          \"type\": \"string\"\n        },\n        \"using_sdk\": {\n          \"description\": \"Using SDK?\",\n          \"type\": \"boolean\"\n        },\n        \"web_job_type\": {\n          \"description\": \"\
  Job type.\",\n          \"enum\": [\n            \"Continuous\",\n            \"Triggered\"\n          ],\n          \"type\": \"string\",\n          \"x-ms-enum\": {\n            \"modelAsString\": false,\n            \"name\": \"WebJobType\"\n          }\n        }\n      },\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-continuous-web-job-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: ContinuousWebJob
---
