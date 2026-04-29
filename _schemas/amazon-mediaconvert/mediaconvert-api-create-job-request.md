---
description: CreateJobRequest schema from Amazon MediaConvert API
layout: schema
name: CreateJobRequest
properties_list:
- description: ''
  name: AccelerationSettings
  type: object
- description: ''
  name: BillingTagsSource
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: HopDestinations
  type: object
- description: ''
  name: JobTemplate
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: Queue
  type: object
- description: ''
  name: Role
  type: object
- description: ''
  name: Settings
  type: object
- description: ''
  name: SimulateReservedQueue
  type: object
- description: ''
  name: StatusUpdateInterval
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: UserMetadata
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-create-job-request-schema.json
slug: mediaconvert-api-create-job-request
source_filename: mediaconvert-api-create-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-job-request-schema.json\",\n  \"title\": \"CreateJobRequest\",\n  \"description\": \"CreateJobRequest schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccelerationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccelerationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accelerationSettings\"\n          },\n          \"description\": \"Optional. Accelerated transcoding can significantly speed up jobs with long, visually complex content. Outputs that use this feature incur pro-tier pricing. For information about feature limitations, see the AWS Elemental MediaConvert User Guide.\"\n        }\n      ]\n    },\n    \"BillingTagsSource\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/BillingTagsSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"billingTagsSource\"\n          },\n          \"description\": \"Optional. Choose a tag type that AWS Billing and Cost Management will use to sort your AWS Elemental MediaConvert costs on any billing report that you set up. Any transcoding outputs that don't have an associated tag will appear in your billing report unsorted. If you don't choose a valid value for this field, your job outputs will appear on the billing report unsorted.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientRequestToken\"\n          },\n          \"description\": \"Prevent duplicate jobs from being created and ensure idempotency for your requests. A client request token can be any string that includes\
  \ up to 64 ASCII characters. If you reuse a client request token within one minute of a successful request, the API returns the job details of the original request instead. For more information see https://docs.aws.amazon.com/mediaconvert/latest/apireference/idempotency.html.\"\n        }\n      ]\n    },\n    \"HopDestinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfHopDestination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hopDestinations\"\n          },\n          \"description\": \"Optional. Use queue hopping to avoid overly long waits in the backlog of the queue that you submit your job to. Specify an alternate queue and the maximum time that your job will wait in the initial queue before hopping. For more information about this feature, see the AWS Elemental MediaConvert User Guide.\"\n        }\n      ]\n    },\n    \"JobTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"jobTemplate\"\n          },\n          \"description\": \"Optional. When you create a job, you can either specify a job template or specify the transcoding settings individually.\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative50Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"priority\"\n          },\n          \"description\": \"Optional. Specify the relative priority for this job. In any given queue, the service begins processing the job with the highest value first. When more than one job has the same priority, the service begins processing the job that you submitted first. If you don't specify a priority, the service uses the default value 0.\"\n        }\n      ]\n    },\n    \"Queue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"queue\"\n          },\n          \"description\": \"Optional. When you create a job, you can specify a queue to send it to. If you don't specify, the job will go to the default queue. For more about queues, see the User Guide topic at https://docs.aws.amazon.com/mediaconvert/latest/ug/what-is.html.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"role\"\n          },\n          \"description\": \"Required. The IAM role you use for creating this job. For details about permissions, see the User Guide topic at the User Guide at https://docs.aws.amazon.com/mediaconvert/latest/ug/iam-role.html.\"\n        }\n      ]\n    },\n    \"Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobSettings\"\n        },\n        {\n          \"xml\": {\n    \
  \        \"name\": \"settings\"\n          },\n          \"description\": \"JobSettings contains all the transcode settings for a job.\"\n        }\n      ]\n    },\n    \"SimulateReservedQueue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulateReservedQueue\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"simulateReservedQueue\"\n          },\n          \"description\": \"Optional. Enable this setting when you run a test job to estimate how many reserved transcoding slots (RTS) you need. When this is enabled, MediaConvert runs your job from an on-demand queue with similar performance to what you will see with one RTS in a reserved queue. This setting is disabled by default.\"\n        }\n      ]\n    },\n    \"StatusUpdateInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusUpdateInterval\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"statusUpdateInterval\"\n\
  \          },\n          \"description\": \"Optional. Specify how often MediaConvert sends STATUS_UPDATE events to Amazon CloudWatch Events. Set the interval, in seconds, between status updates. MediaConvert sends an update at this interval from the time the service begins processing your job to the time it completes the transcode or encounters an error.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"Optional. The tags that you want to add to the resource. You can tag resources with a key-value pair or with only a key.  Use standard AWS tags on your job for automatic integration with AWS services and for custom integrations and workflows.\"\n        }\n      ]\n    },\n    \"UserMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"userMetadata\"\n          },\n          \"description\": \"Optional. User-defined metadata that you want to associate with an MediaConvert job. You specify metadata in key/value pairs.  Use only for existing integrations or workflows that rely on job metadata tags. Otherwise, we recommend that you use standard AWS tags.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Role\",\n    \"Settings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-job-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateJobRequest
---
