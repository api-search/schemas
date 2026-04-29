---
description: BatchDeleteConfigurationTask schema from Amazon Application Discovery Service API
layout: schema
name: BatchDeleteConfigurationTask
properties_list:
- description: The deletion task's unique identifier.
  name: taskId
  type: string
- description: The current execution status of the deletion task.
  name: status
  type: string
- description: An epoch seconds timestamp (Unix) of when the deletion task was started.
  name: startTime
  type: string
- description: An epoch seconds timestamp (Unix) of when the deletion task was completed.
  name: endTime
  type: string
- description: The type of configuration item to delete.
  name: configurationType
  type: string
- description: The list of configuration IDs that were originally requested to be deleted by this task.
  name: requestedConfigurations
  type: array
- description: The list of configuration IDs that were successfully deleted by this task.
  name: deletedConfigurations
  type: array
- description: A list of configuration IDs that produced an associated error.
  name: failedConfigurations
  type: array
- description: A list of warnings associated with this deletion task.
  name: deletionWarnings
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-batch-delete-configuration-task-schema.json
slug: application-discovery-service-batch-delete-configuration-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-configuration-task-schema.json\",\n  \"title\": \"BatchDeleteConfigurationTask\",\n  \"description\": \"BatchDeleteConfigurationTask schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"type\": \"string\",\n      \"example\": \"task-500123\",\n      \"description\": \"The deletion task's unique identifier.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INITIALIZING\",\n        \"VALIDATING\",\n        \"DELETING\",\n        \"COMPLETED\",\n        \"FAILED\"\n      ],\n      \"example\": \"COMPLETED\",\n      \"description\": \"The current execution status of the deletion task.\"\n    },\n    \"startTime\": {\n      \"type\"\
  : \"string\",\n      \"example\": \"2026-04-19T10:00:00Z\",\n      \"description\": \"An epoch seconds timestamp (Unix) of when the deletion task was started.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-19T10:05:00Z\",\n      \"description\": \"An epoch seconds timestamp (Unix) of when the deletion task was completed.\"\n    },\n    \"configurationType\": {\n      \"type\": \"string\",\n      \"example\": \"SERVER\",\n      \"description\": \"The type of configuration item to delete.\"\n    },\n    \"requestedConfigurations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-SERVER-500456\"\n      ],\n      \"description\": \"The list of configuration IDs that were originally requested to be deleted by this task.\"\n    },\n    \"deletedConfigurations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n\
  \        \"d-SERVER-500456\"\n      ],\n      \"description\": \"The list of configuration IDs that were successfully deleted by this task.\"\n    },\n    \"failedConfigurations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"configurationId\": {\n            \"type\": \"string\",\n            \"example\": \"d-SERVER-500456\",\n            \"description\": \"The configuration ID of the configuration that failed to delete.\"\n          },\n          \"errorStatusCode\": {\n            \"type\": \"integer\",\n            \"example\": 404,\n            \"description\": \"The error status code.\"\n          },\n          \"errorMessage\": {\n            \"type\": \"string\",\n            \"example\": \"Configuration item not found\",\n            \"description\": \"A descriptive message indicating why the associated configuration failed to delete.\"\n          }\n        }\n      },\n      \"description\": \"A list\
  \ of configuration IDs that produced an associated error.\"\n    },\n    \"deletionWarnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"configurationId\": {\n            \"type\": \"string\",\n            \"example\": \"d-SERVER-500456\",\n            \"description\": \"The configuration ID of the configuration item associated with the deletion warning.\"\n          },\n          \"warningCode\": {\n            \"type\": \"integer\",\n            \"example\": 1,\n            \"description\": \"The integer warning code associated with the warning message.\"\n          },\n          \"warningText\": {\n            \"type\": \"string\",\n            \"example\": \"Configuration item may have dependencies\",\n            \"description\": \"A descriptive message of the warning the associated configuration item produced.\"\n          }\n        }\n      },\n      \"description\": \"A list of warnings associated with\
  \ this deletion task.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-configuration-task-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: BatchDeleteConfigurationTask
---
