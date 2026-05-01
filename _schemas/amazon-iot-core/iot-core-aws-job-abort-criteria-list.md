---
description: AwsJobAbortCriteriaList schema
layout: schema
name: AwsJobAbortCriteriaList
properties_list: []
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-aws-job-abort-criteria-list-schema.json
slug: iot-core-aws-job-abort-criteria-list
source_filename: iot-core-aws-job-abort-criteria-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-aws-job-abort-criteria-list-schema.json\",\n  \"title\": \"AwsJobAbortCriteriaList\",\n  \"description\": \"AwsJobAbortCriteriaList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"failureType\",\n      \"action\",\n      \"thresholdPercentage\",\n      \"minNumberOfExecutedThings\"\n    ],\n    \"properties\": {\n      \"failureType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AwsJobAbortCriteriaFailureType\"\n          },\n          {\n            \"description\": \"The type of job execution failures that can initiate a job abort.\"\n          }\n        ]\n      },\n      \"action\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AwsJobAbortCriteriaAbortAction\"\
  \n          },\n          {\n            \"description\": \"The type of job action to take to initiate the job abort.\"\n          }\n        ]\n      },\n      \"thresholdPercentage\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AwsJobAbortCriteriaAbortThresholdPercentage\"\n          },\n          {\n            \"description\": \"<p>The minimum percentage of job execution failures that must occur to initiate the job abort.</p> <p>Amazon Web Services IoT Core supports up to two digits after the decimal (for example, 10.9 and 10.99, but not 10.999).</p>\"\n          }\n        ]\n      },\n      \"minNumberOfExecutedThings\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AwsJobAbortCriteriaMinimumNumberOfExecutedThings\"\n          },\n          {\n            \"description\": \"The minimum number of things which must receive job execution notifications before the job can be aborted.\"\n          }\n        ]\n\
  \      }\n    },\n    \"description\": \"The criteria that determine when and how a job abort takes place.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-aws-job-abort-criteria-list-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: AwsJobAbortCriteriaList
---
