---
description: UpdateJobTemplateRequest schema from Amazon MediaConvert API
layout: schema
name: UpdateJobTemplateRequest
properties_list:
- description: ''
  name: AccelerationSettings
  type: object
- description: ''
  name: Category
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: HopDestinations
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: Queue
  type: object
- description: ''
  name: Settings
  type: object
- description: ''
  name: StatusUpdateInterval
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-update-job-template-request-schema.json
slug: mediaconvert-api-update-job-template-request
source_filename: mediaconvert-api-update-job-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-update-job-template-request-schema.json\",\n  \"title\": \"UpdateJobTemplateRequest\",\n  \"description\": \"UpdateJobTemplateRequest schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccelerationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccelerationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accelerationSettings\"\n          },\n          \"description\": \"Accelerated transcoding can significantly speed up jobs with long, visually complex content. Outputs that use this feature incur pro-tier pricing. For information about feature limitations, see the AWS Elemental MediaConvert User Guide.\"\n        }\n      ]\n    },\n    \"Category\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"category\"\n          },\n          \"description\": \"The new category for the job template, if you are changing it.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"The new description for the job template, if you are changing it.\"\n        }\n      ]\n    },\n    \"HopDestinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfHopDestination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hopDestinations\"\n          },\n          \"description\": \"Optional list of hop destinations.\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__integerMinNegative50Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"priority\"\n          },\n          \"description\": \"Specify the relative priority for this job. In any given queue, the service begins processing the job with the highest value first. When more than one job has the same priority, the service begins processing the job that you submitted first. If you don't specify a priority, the service uses the default value 0.\"\n        }\n      ]\n    },\n    \"Queue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"queue\"\n          },\n          \"description\": \"The new queue for the job template, if you are changing it.\"\n        }\n      ]\n    },\n    \"Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTemplateSettings\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"settings\"\n          },\n          \"description\": \"JobTemplateSettings contains all the transcode settings saved in the template that will be applied to jobs created from it.\"\n        }\n      ]\n    },\n    \"StatusUpdateInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusUpdateInterval\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"statusUpdateInterval\"\n          },\n          \"description\": \"Specify how often MediaConvert sends STATUS_UPDATE events to Amazon CloudWatch Events. Set the interval, in seconds, between status updates. MediaConvert sends an update at this interval from the time the service begins processing your job to the time it completes the transcode or encounters an error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-update-job-template-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateJobTemplateRequest
---
