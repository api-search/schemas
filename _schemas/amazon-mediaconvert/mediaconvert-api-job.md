---
description: Each job converts an input file into an output file or files. For more information, see the User Guide at https://docs.aws.amazon.com/mediaconvert/latest/ug/what-is.html
layout: schema
name: Job
properties_list:
- description: ''
  name: AccelerationSettings
  type: object
- description: ''
  name: AccelerationStatus
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: BillingTagsSource
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: CurrentPhase
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: HopDestinations
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: JobPercentComplete
  type: object
- description: ''
  name: JobTemplate
  type: object
- description: ''
  name: Messages
  type: object
- description: ''
  name: OutputGroupDetails
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: Queue
  type: object
- description: ''
  name: QueueTransitions
  type: object
- description: ''
  name: RetryCount
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
  name: Status
  type: object
- description: ''
  name: StatusUpdateInterval
  type: object
- description: ''
  name: Timing
  type: object
- description: ''
  name: UserMetadata
  type: object
- description: ''
  name: Warnings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-job-schema.json
slug: mediaconvert-api-job
source_filename: mediaconvert-api-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"Each job converts an input file into an output file or files. For more information, see the User Guide at https://docs.aws.amazon.com/mediaconvert/latest/ug/what-is.html\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccelerationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccelerationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accelerationSettings\"\n          },\n          \"description\": \"Accelerated transcoding can significantly speed up jobs with long, visually complex content.\"\n        }\n      ]\n    },\n    \"AccelerationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccelerationStatus\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"accelerationStatus\"\n          },\n          \"description\": \"Describes whether the current job is running with accelerated transcoding. For jobs that have Acceleration (AccelerationMode) set to DISABLED, AccelerationStatus is always NOT_APPLICABLE. For jobs that have Acceleration (AccelerationMode) set to ENABLED or PREFERRED, AccelerationStatus is one of the other states. AccelerationStatus is IN_PROGRESS initially, while the service determines whether the input files and job settings are compatible with accelerated transcoding. If they are, AcclerationStatus is ACCELERATED. If your input files and job settings aren't compatible with accelerated transcoding, the service either fails your job or runs it without accelerated transcoding, depending on how you set Acceleration (AccelerationMode). When the service runs your job without accelerated transcoding, AccelerationStatus is NOT_ACCELERATED.\"\n        }\n   \
  \   ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"An identifier for this resource that is unique within all of AWS.\"\n        }\n      ]\n    },\n    \"BillingTagsSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingTagsSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"billingTagsSource\"\n          },\n          \"description\": \"The tag type that AWS Billing and Cost Management will use to sort your AWS Elemental MediaConvert costs on any billing report that you set up.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientRequestToken\"\n          },\n          \"\
  description\": \"Prevent duplicate jobs from being created and ensure idempotency for your requests. A client request token can be any string that includes up to 64 ASCII characters. If you reuse a client request token within one minute of a successful request, the API returns the job details of the original request instead. For more information see https://docs.aws.amazon.com/mediaconvert/latest/apireference/idempotency.html.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The time, in Unix epoch format in seconds, when the job got created.\"\n        }\n      ]\n    },\n    \"CurrentPhase\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobPhase\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentPhase\"\n \
  \         },\n          \"description\": \"A job's phase can be PROBING, TRANSCODING OR UPLOADING\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"errorCode\"\n          },\n          \"description\": \"Error code for the job\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"errorMessage\"\n          },\n          \"description\": \"Error message of Job\"\n        }\n      ]\n    },\n    \"HopDestinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfHopDestination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hopDestinations\"\n          },\n          \"description\": \"Optional list of hop destinations.\"\
  \n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"A portion of the job's ARN, unique within your AWS Elemental MediaConvert resources\"\n        }\n      ]\n    },\n    \"JobPercentComplete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"jobPercentComplete\"\n          },\n          \"description\": \"An estimate of how far your job has progressed. This estimate is shown as a percentage of the total time from when your job leaves its queue to when your output files appear in your output Amazon S3 bucket. AWS Elemental MediaConvert provides jobPercentComplete in CloudWatch STATUS_UPDATE events and in the response to GetJob and ListJobs requests. The jobPercentComplete estimate is\
  \ reliable for the following input containers: Quicktime, Transport Stream, MP4, and MXF. For some jobs, the service can't provide information about job progress. In those cases, jobPercentComplete returns a null value.\"\n        }\n      ]\n    },\n    \"JobTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"jobTemplate\"\n          },\n          \"description\": \"The job template that the job is created from, if it is created from a job template.\"\n        }\n      ]\n    },\n    \"Messages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobMessages\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"messages\"\n          },\n          \"description\": \"Provides messages from the service about jobs that you have already successfully submitted.\"\n        }\n      ]\n    },\n    \"OutputGroupDetails\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutputGroupDetail\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputGroupDetails\"\n          },\n          \"description\": \"List of output group details\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative50Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"priority\"\n          },\n          \"description\": \"Relative priority on the job.\"\n        }\n      ]\n    },\n    \"Queue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"queue\"\n          },\n          \"description\": \"When you create a job, you can specify a queue to send it to. If you don't specify, the job will go to the default queue. For more about queues, see the User Guide topic at https://docs.aws.amazon.com/mediaconvert/latest/ug/what-is.html\"\
  \n        }\n      ]\n    },\n    \"QueueTransitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfQueueTransition\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"queueTransitions\"\n          },\n          \"description\": \"The job's queue hopping history.\"\n        }\n      ]\n    },\n    \"RetryCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"retryCount\"\n          },\n          \"description\": \"The number of times that the service automatically attempted to process your job after encountering an error.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"role\"\n          },\n          \"description\": \"The IAM role you use for creating this job.\
  \ For details about permissions, see the User Guide topic at the User Guide at https://docs.aws.amazon.com/mediaconvert/latest/ug/iam-role.html\"\n        }\n      ]\n    },\n    \"Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"settings\"\n          },\n          \"description\": \"JobSettings contains all the transcode settings for a job.\"\n        }\n      ]\n    },\n    \"SimulateReservedQueue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulateReservedQueue\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"simulateReservedQueue\"\n          },\n          \"description\": \"Enable this setting when you run a test job to estimate how many reserved transcoding slots (RTS) you need. When this is enabled, MediaConvert runs your job from an on-demand queue with similar performance to what you will see with\
  \ one RTS in a reserved queue. This setting is disabled by default.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"A job's status can be SUBMITTED, PROGRESSING, COMPLETE, CANCELED, or ERROR.\"\n        }\n      ]\n    },\n    \"StatusUpdateInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusUpdateInterval\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"statusUpdateInterval\"\n          },\n          \"description\": \"Specify how often MediaConvert sends STATUS_UPDATE events to Amazon CloudWatch Events. Set the interval, in seconds, between status updates. MediaConvert sends an update at this interval from the time the service begins processing your job to the time it completes the transcode or encounters an error.\"\
  \n        }\n      ]\n    },\n    \"Timing\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timing\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timing\"\n          },\n          \"description\": \"Information about when jobs are submitted, started, and finished is specified in Unix epoch format in seconds.\"\n        }\n      ]\n    },\n    \"UserMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userMetadata\"\n          },\n          \"description\": \"User-defined metadata that you want to associate with an MediaConvert job. You specify metadata in key/value pairs.\"\n        }\n      ]\n    },\n    \"Warnings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfWarningGroup\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"warnings\"\n         \
  \ },\n          \"description\": \"Contains any warning messages for the job. Use to help identify potential issues with your input, output, or job. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/warning_codes.html\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Settings\",\n    \"Role\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Job
---
