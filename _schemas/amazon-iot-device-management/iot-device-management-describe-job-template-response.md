---
description: DescribeJobTemplateResponse schema
layout: schema
name: DescribeJobTemplateResponse
properties_list:
- description: ''
  name: jobTemplateArn
  type: object
- description: ''
  name: jobTemplateId
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: documentSource
  type: object
- description: ''
  name: document
  type: object
- description: ''
  name: createdAt
  type: object
- description: Configuration for pre-signed S3 URLs.
  name: presignedUrlConfig
  type: object
- description: Allows you to create a staged rollout of a job.
  name: jobExecutionsRolloutConfig
  type: object
- description: The criteria that determine when and how a job abort takes place.
  name: abortConfig
  type: object
- description: Specifies the amount of time each device has to finish its execution of the job. A timer is started when the job execution status is set to <code>IN_PROGRESS</code>. If the job execution status is not
  name: timeoutConfig
  type: object
- description: ''
  name: jobExecutionsRetryConfig
  type: object
- description: ''
  name: maintenanceWindows
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-job-template-response-schema.json
slug: iot-device-management-describe-job-template-response
source_filename: iot-device-management-describe-job-template-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-job-template-response-schema.json\",\n  \"title\": \"DescribeJobTemplateResponse\",\n  \"description\": \"DescribeJobTemplateResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobTemplateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTemplateArn\"\n        },\n        {\n          \"description\": \"The ARN of the job template.\"\n        }\n      ]\n    },\n    \"jobTemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTemplateId\"\n        },\n        {\n          \"description\": \"The unique identifier of the job template.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDescription\"\
  \n        },\n        {\n          \"description\": \"A description of the job template.\"\n        }\n      ]\n    },\n    \"documentSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDocumentSource\"\n        },\n        {\n          \"description\": \"An S3 link to the job document.\"\n        }\n      ]\n    },\n    \"document\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDocument\"\n        },\n        {\n          \"description\": \"The job document.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The time, in seconds since the epoch, when the job template was created.\"\n        }\n      ]\n    },\n    \"presignedUrlConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"roleArn\": {\n          \"allOf\": [\n            {\n              \"$ref\"\
  : \"#/components/schemas/RoleArn\"\n            },\n            {\n              \"description\": \"<p>The ARN of an IAM role that grants grants permission to download files from the S3 bucket where the job data/updates are stored. The role must also grant permission for IoT to download the files.</p> <important> <p>For information about addressing the confused deputy problem, see <a href=\\\"https://docs.aws.amazon.com/iot/latest/developerguide/cross-service-confused-deputy-prevention.html\\\">cross-service confused deputy prevention</a> in the <i>Amazon Web Services IoT Core developer guide</i>.</p> </important>\"\n            }\n          ]\n        },\n        \"expiresInSec\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ExpiresInSec\"\n            },\n            {\n              \"description\": \"How long (in seconds) pre-signed URLs are valid. Valid values are 60 - 3600, the default value is 3600 seconds. Pre-signed URLs are generated\
  \ when Jobs receives an MQTT request for the job document.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Configuration for pre-signed S3 URLs.\"\n    },\n    \"jobExecutionsRolloutConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"maximumPerMinute\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/MaxJobExecutionsPerMin\"\n            },\n            {\n              \"description\": \"The maximum number of things that will be notified of a pending job, per minute. This parameter allows you to create a staged rollout.\"\n            }\n          ]\n        },\n        \"exponentialRate\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ExponentialRolloutRate\"\n            },\n            {\n              \"description\": \"The rate of increase for a job rollout. This parameter allows you to define an exponential rate for a job rollout.\"\n        \
  \    }\n          ]\n        }\n      },\n      \"description\": \"Allows you to create a staged rollout of a job.\"\n    },\n    \"abortConfig\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"criteriaList\"\n      ],\n      \"properties\": {\n        \"criteriaList\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/AbortCriteriaList\"\n            },\n            {\n              \"description\": \"The list of criteria that determine when and how to abort the job.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"The criteria that determine when and how a job abort takes place.\"\n    },\n    \"timeoutConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"inProgressTimeoutInMinutes\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/InProgressTimeoutInMinutes\"\n            },\n            {\n              \"description\": \"Specifies the\
  \ amount of time, in minutes, this device has to finish execution of this job. The timeout interval can be anywhere between 1 minute and 7 days (1 to 10080 minutes). The in progress timer can't be updated and will apply to all job executions for the job. Whenever a job execution remains in the IN_PROGRESS status for longer than this interval, the job execution will fail and switch to the terminal <code>TIMED_OUT</code> status.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Specifies the amount of time each device has to finish its execution of the job. A timer is started when the job execution status is set to <code>IN_PROGRESS</code>. If the job execution status is not set to another terminal state before the timer expires, it will be automatically set to <code>TIMED_OUT</code>.\"\n    },\n    \"jobExecutionsRetryConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobExecutionsRetryConfig\"\n        },\n        {\n     \
  \     \"description\": \"The configuration that determines how many retries are allowed for each failure type for a job.\"\n        }\n      ]\n    },\n    \"maintenanceWindows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaintenanceWindows\"\n        },\n        {\n          \"description\": \"Allows you to configure an optional maintenance window for the rollout of a job document to all devices in the target group for a job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-job-template-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeJobTemplateResponse
---
