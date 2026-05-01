---
description: Provides information about a targeted sentiment detection job.
layout: schema
name: TargetedSentimentDetectionJobProperties
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
  name: VolumeKmsKeyId
  type: object
- description: ''
  name: VpcConfig
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-targeted-sentiment-detection-job-properties-schema.json
slug: openapi.yml-targeted-sentiment-detection-job-properties
source_filename: openapi.yml-targeted-sentiment-detection-job-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-targeted-sentiment-detection-job-properties-schema.json\",\n  \"title\": \"TargetedSentimentDetectionJobProperties\",\n  \"description\": \"Provides information about a targeted sentiment detection job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The identifier assigned to the targeted sentiment detection job.\"\n        }\n      ]\n    },\n    \"JobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the targeted sentiment detection job. It is a unique, fully qualified identifier for the job. It includes\
  \ the Amazon Web Services account, Amazon Web Services Region, and the job ID. The format of the ARN is as follows:</p> <p> <code>arn:&lt;partition&gt;:comprehend:&lt;region&gt;:&lt;account-id&gt;:targeted-sentiment-detection-job/&lt;job-id&gt;</code> </p> <p>The following is an example job ARN:</p> <p> <code>arn:aws:comprehend:us-west-2:111122223333:targeted-sentiment-detection-job/1234abcd12ab34cd56ef1234567890ab</code> </p>\"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The name that you assigned to the targeted sentiment detection job.\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The current status of the targeted sentiment detection job. If the status is <code>FAILED</code>, the <code>Messages</code>\
  \ field shows the reason for the failure.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnyLengthString\"\n        },\n        {\n          \"description\": \"A description of the status of a job.\"\n        }\n      ]\n    },\n    \"SubmitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the targeted sentiment detection job was submitted for processing.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the targeted sentiment detection job ended.\"\n        }\n      ]\n    },\n    \"InputDataConfig\": {\n      \"$ref\": \"#/components/schemas/InputDataConfig\"\n    },\n    \"OutputDataConfig\": {\n      \"$ref\": \"#/components/schemas/OutputDataConfig\"\
  \n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"The language code of the input documents.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend read access to your input data.\"\n        }\n      ]\n    },\n    \"VolumeKmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"<p>ID for the KMS key that Amazon Comprehend uses to encrypt the data on the storage volume attached to the ML compute instance(s) that process the targeted sentiment detection job. The VolumeKmsKeyId can be either of the following formats:</p> <ul> <li> <p>KMS Key ID: <code>\\\
  \"1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> <li> <p>Amazon Resource Name (ARN) of a KMS Key: <code>\\\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"VpcConfig\": {\n      \"$ref\": \"#/components/schemas/VpcConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-targeted-sentiment-detection-job-properties-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: TargetedSentimentDetectionJobProperties
---
