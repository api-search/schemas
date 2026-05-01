---
description: A job template is a pre-made set of encoding instructions that you can use to quickly create a job.
layout: schema
name: JobTemplate
properties_list:
- description: ''
  name: AccelerationSettings
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: Category
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: HopDestinations
  type: object
- description: ''
  name: LastUpdated
  type: object
- description: ''
  name: Name
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
- description: ''
  name: Type
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-job-template-schema.json
slug: mediaconvert-api-job-template
source_filename: mediaconvert-api-job-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-template-schema.json\",\n  \"title\": \"JobTemplate\",\n  \"description\": \"A job template is a pre-made set of encoding instructions that you can use to quickly create a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccelerationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccelerationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accelerationSettings\"\n          },\n          \"description\": \"Accelerated transcoding can significantly speed up jobs with long, visually complex content.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"\
  arn\"\n          },\n          \"description\": \"An identifier for this resource that is unique within all of AWS.\"\n        }\n      ]\n    },\n    \"Category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"category\"\n          },\n          \"description\": \"An optional category you create to organize your job templates.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The timestamp in epoch seconds for Job template creation.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n   \
  \       },\n          \"description\": \"An optional description you create for each job template.\"\n        }\n      ]\n    },\n    \"HopDestinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfHopDestination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hopDestinations\"\n          },\n          \"description\": \"Optional list of hop destinations.\"\n        }\n      ]\n    },\n    \"LastUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lastUpdated\"\n          },\n          \"description\": \"The timestamp in epoch seconds when the Job template was last updated.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n    \
  \      \"description\": \"A name you create for each job template. Each name must be unique within your account.\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative50Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"priority\"\n          },\n          \"description\": \"Relative priority on the job.\"\n        }\n      ]\n    },\n    \"Queue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"queue\"\n          },\n          \"description\": \"Optional. The queue that jobs created from this template are assigned to. If you don't specify this, jobs will go to the default queue.\"\n        }\n      ]\n    },\n    \"Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTemplateSettings\"\n        },\n        {\n          \"\
  xml\": {\n            \"name\": \"settings\"\n          },\n          \"description\": \"JobTemplateSettings contains all the transcode settings saved in the template that will be applied to jobs created from it.\"\n        }\n      ]\n    },\n    \"StatusUpdateInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusUpdateInterval\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"statusUpdateInterval\"\n          },\n          \"description\": \"Specify how often MediaConvert sends STATUS_UPDATE events to Amazon CloudWatch Events. Set the interval, in seconds, between status updates. MediaConvert sends an update at this interval from the time the service begins processing your job to the time it completes the transcode or encounters an error.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Type\"\n        },\n        {\n          \"xml\": {\n          \
  \  \"name\": \"type\"\n          },\n          \"description\": \"A job template can be of two types: system or custom. System or built-in job templates can't be modified or deleted by the user.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Settings\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-template-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: JobTemplate
---
