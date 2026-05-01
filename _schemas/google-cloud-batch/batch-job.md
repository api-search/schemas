---
description: Represents a Batch job resource, including its task groups, allocation policy, status, and scheduling configuration.
layout: schema
name: Google Cloud Batch Job
properties_list:
- description: The resource name of the job.
  name: name
  type: string
- description: A system generated unique ID for the job.
  name: uid
  type: string
- description: Priority of the job. Higher values indicate higher priority.
  name: priority
  type: string
- description: Required. TaskGroups in the job.
  name: taskGroups
  type: array
- description: Compute resource allocation for the job.
  name: allocationPolicy
  type: object
- description: Current status of the job.
  name: status
  type: object
- description: When the job was created.
  name: createTime
  type: string
- description: The last time the job was updated.
  name: updateTime
  type: string
provider_name: Google Cloud Batch
provider_slug: google-cloud-batch
schema_file: json-schema/batch-job.json
slug: batch-job
source_filename: batch-job.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/google-cloud-batch/refs/heads/main/json-schema/batch-job.json\",\n  \"title\": \"Google Cloud Batch Job\",\n  \"description\": \"Represents a Batch job resource, including its task groups, allocation policy, status, and scheduling configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the job.\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"A system generated unique ID for the job.\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Priority of the job. Higher values indicate higher priority.\"\n    },\n    \"taskGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Required. TaskGroups in the job.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"taskSpec\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"runnables\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"script\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"text\": {\n                          \"type\": \"string\"\n                        }\n                      }\n                    },\n                    \"container\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"imageUri\": {\n                          \"type\": \"string\"\n                        },\n                        \"commands\": {\n                          \"type\": \"array\",\n                          \"items\": {\n\
  \                            \"type\": \"string\"\n                          }\n                        }\n                      }\n                    }\n                  }\n                }\n              },\n              \"maxRunDuration\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"taskCount\": {\n            \"type\": \"string\"\n          },\n          \"parallelism\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"allocationPolicy\": {\n      \"type\": \"object\",\n      \"description\": \"Compute resource allocation for the job.\",\n      \"properties\": {\n        \"location\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"allowedLocations\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"instances\": {\n          \"type\": \"\
  array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"policy\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"machineType\": {\n                    \"type\": \"string\"\n                  },\n                  \"provisioningModel\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"description\": \"Current status of the job.\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"STATE_UNSPECIFIED\",\n            \"QUEUED\",\n            \"SCHEDULED\",\n            \"RUNNING\",\n            \"SUCCEEDED\",\n            \"FAILED\",\n            \"DELETION_IN_PROGRESS\"\n          ]\n        },\n        \"runDuration\": {\n          \"type\": \"string\"\
  \n        }\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the job was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last time the job was updated.\"\n    }\n  },\n  \"required\": [\"taskGroups\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-batch/refs/heads/main/json-schema/batch-job.json
tags:
- Batch Processing
- Compute
- Google Cloud
- HPC
- Jobs
title: Google Cloud Batch Job
---
