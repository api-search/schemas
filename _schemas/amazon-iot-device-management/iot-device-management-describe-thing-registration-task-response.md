---
description: DescribeThingRegistrationTaskResponse schema
layout: schema
name: DescribeThingRegistrationTaskResponse
properties_list:
- description: ''
  name: taskId
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastModifiedDate
  type: object
- description: ''
  name: templateBody
  type: object
- description: ''
  name: inputFileBucket
  type: object
- description: ''
  name: inputFileKey
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: successCount
  type: object
- description: ''
  name: failureCount
  type: object
- description: ''
  name: percentageProgress
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-thing-registration-task-response-schema.json
slug: iot-device-management-describe-thing-registration-task-response
source_filename: iot-device-management-describe-thing-registration-task-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-thing-registration-task-response-schema.json\",\n  \"title\": \"DescribeThingRegistrationTaskResponse\",\n  \"description\": \"DescribeThingRegistrationTaskResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskId\"\n        },\n        {\n          \"description\": \"The task ID.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreationDate\"\n        },\n        {\n          \"description\": \"The task creation date.\"\n        }\n      ]\n    },\n    \"lastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedDate\"\n  \
  \      },\n        {\n          \"description\": \"The date when the task was last modified.\"\n        }\n      ]\n    },\n    \"templateBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateBody\"\n        },\n        {\n          \"description\": \"The task's template.\"\n        }\n      ]\n    },\n    \"inputFileBucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistryS3BucketName\"\n        },\n        {\n          \"description\": \"The S3 bucket that contains the input file.\"\n        }\n      ]\n    },\n    \"inputFileKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistryS3KeyName\"\n        },\n        {\n          \"description\": \"The input file key.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The role ARN that grants\
  \ access to the input file bucket.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The status of the bulk thing provisioning task.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \"The message.\"\n        }\n      ]\n    },\n    \"successCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The number of things successfully provisioned.\"\n        }\n      ]\n    },\n    \"failureCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The number of things that failed to be provisioned.\"\n        }\n      ]\n    },\n    \"percentageProgress\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The progress of the bulk provisioning task expressed as a percentage.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-thing-registration-task-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeThingRegistrationTaskResponse
---
