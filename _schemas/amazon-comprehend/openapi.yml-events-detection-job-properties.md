---
description: Provides information about an events detection job.
layout: schema
name: EventsDetectionJobProperties
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobArn
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobStatus
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: SubmitTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: InputDataConfig
  type: object
- description: ''
  name: OutputDataConfig
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: TargetEventTypes
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-events-detection-job-properties-schema.json
slug: openapi.yml-events-detection-job-properties
source_filename: openapi.yml-events-detection-job-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-events-detection-job-properties-schema.json\",\n  \"title\": \"EventsDetectionJobProperties\",\n  \"description\": \"Provides information about an events detection job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The identifier assigned to the events detection job.\"\n        }\n      ]\n    },\n    \"JobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the events detection job. It is a unique, fully qualified identifier for the job. It includes the Amazon Web Services account, Amazon Web Services\
  \ Region, and the job ID. The format of the ARN is as follows:</p> <p> <code>arn:&lt;partition&gt;:comprehend:&lt;region&gt;:&lt;account-id&gt;:events-detection-job/&lt;job-id&gt;</code> </p> <p>The following is an example job ARN:</p> <p> <code>arn:aws:comprehend:us-west-2:111122223333:events-detection-job/1234abcd12ab34cd56ef1234567890ab</code> </p>\"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The name you assigned the events detection job.\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The current status of the events detection job.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnyLengthString\"\n        },\n        {\n  \
  \        \"description\": \"A description of the status of the events detection job.\"\n        }\n      ]\n    },\n    \"SubmitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the events detection job was submitted for processing.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the events detection job completed.\"\n        }\n      ]\n    },\n    \"InputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDataConfig\"\n        },\n        {\n          \"description\": \"The input data configuration that you supplied when you created the events detection job.\"\n        }\n      ]\n    },\n    \"OutputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputDataConfig\"\
  \n        },\n        {\n          \"description\": \"The output data configuration that you supplied when you created the events detection job.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"The language code of the input documents.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend read access to your input data.\"\n        }\n      ]\n    },\n    \"TargetEventTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetEventTypes\"\n        },\n        {\n          \"description\": \"The types of events that are detected by the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-events-detection-job-properties-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EventsDetectionJobProperties
---
