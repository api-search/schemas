---
description: StartEventsDetectionJobRequest schema
layout: schema
name: StartEventsDetectionJobRequest
properties_list:
- description: ''
  name: InputDataConfig
  type: object
- description: ''
  name: OutputDataConfig
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: TargetEventTypes
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-start-events-detection-job-request-schema.json
slug: openapi.yml-start-events-detection-job-request
source_filename: openapi.yml-start-events-detection-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-start-events-detection-job-request-schema.json\",\n  \"title\": \"StartEventsDetectionJobRequest\",\n  \"description\": \"StartEventsDetectionJobRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDataConfig\"\n        },\n        {\n          \"description\": \"Specifies the format and location of the input data for the job.\"\n        }\n      ]\n    },\n    \"OutputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputDataConfig\"\n        },\n        {\n          \"description\": \"Specifies where to send the output files.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend read access to your input data.\"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The identifier of the events detection job.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"The language code of the input documents.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\": \"An unique identifier for the request. If you don't set the client request token, Amazon Comprehend generates\
  \ one.\"\n        }\n      ]\n    },\n    \"TargetEventTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetEventTypes\"\n        },\n        {\n          \"description\": \"The types of events to detect in the input documents.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Tags to associate with the events detection job. A tag is a key-value pair that adds metadata to a resource used by Amazon Comprehend. For example, a tag with \\\"Sales\\\" as the key might be added to a resource to indicate its use by the sales department.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InputDataConfig\",\n    \"OutputDataConfig\",\n    \"DataAccessRoleArn\",\n    \"LanguageCode\",\n    \"TargetEventTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-start-events-detection-job-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: StartEventsDetectionJobRequest
---
