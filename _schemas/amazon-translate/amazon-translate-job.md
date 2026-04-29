---
description: Schema representing an Amazon Translate batch translation job resource.
layout: schema
name: Amazon Translate Translation Job
properties_list:
- description: The ID of the translation job.
  name: JobId
  type: string
- description: The user-provided name of the translation job.
  name: JobName
  type: string
- description: The status of the translation job.
  name: JobStatus
  type: string
- description: The language code of the source language.
  name: SourceLanguageCode
  type: string
- description: The language codes of the target languages.
  name: TargetLanguageCodes
  type: array
- description: The input data configuration for the translation job.
  name: InputDataConfig
  type: object
- description: The output data configuration for the translation job.
  name: OutputDataConfig
  type: object
- description: The Amazon Resource Name (ARN) of the IAM role for S3 access.
  name: DataAccessRoleArn
  type: string
- description: The names of custom terminologies applied to the job.
  name: TerminologyNames
  type: array
- description: The time the translation job was submitted.
  name: SubmittedTime
  type: string
- description: The time the translation job ended.
  name: EndTime
  type: string
- description: A list of tags associated with the translation job.
  name: Tags
  type: array
provider_name: Amazon Translate
provider_slug: amazon-translate
schema_file: json-schema/amazon-translate-job-schema.json
slug: amazon-translate-job
source_filename: amazon-translate-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://translate.amazonaws.com/schemas/translation-job\",\n  \"title\": \"Amazon Translate Translation Job\",\n  \"description\": \"Schema representing an Amazon Translate batch translation job resource.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"InputDataConfig\",\n    \"OutputDataConfig\",\n    \"DataAccessRoleArn\",\n    \"SourceLanguageCode\",\n    \"TargetLanguageCodes\"\n  ],\n  \"properties\": {\n    \"JobId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the translation job.\",\n      \"minLength\": 1,\n      \"maxLength\": 32,\n      \"pattern\": \"^[a-zA-Z0-9-]+$\"\n    },\n    \"JobName\": {\n      \"type\": \"string\",\n      \"description\": \"The user-provided name of the translation job.\",\n      \"minLength\": 1,\n      \"maxLength\": 256,\n      \"pattern\": \"^[\\\\P{M}\\\\p{M}]{1,256}$\"\n    },\n    \"JobStatus\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The status of the translation job.\",\n      \"enum\": [\n        \"SUBMITTED\",\n        \"IN_PROGRESS\",\n        \"COMPLETED\",\n        \"COMPLETED_WITH_ERROR\",\n        \"FAILED\",\n        \"STOP_REQUESTED\",\n        \"STOPPED\"\n      ]\n    },\n    \"SourceLanguageCode\": {\n      \"type\": \"string\",\n      \"description\": \"The language code of the source language.\",\n      \"minLength\": 2,\n      \"maxLength\": 5\n    },\n    \"TargetLanguageCodes\": {\n      \"type\": \"array\",\n      \"description\": \"The language codes of the target languages.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"minLength\": 2,\n        \"maxLength\": 5\n      },\n      \"minItems\": 1\n    },\n    \"InputDataConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The input data configuration for the translation job.\",\n      \"required\": [\n        \"S3Uri\",\n        \"ContentType\"\n      ],\n      \"properties\": {\n       \
  \ \"S3Uri\": {\n          \"type\": \"string\",\n          \"description\": \"The URI of the S3 folder containing the input documents.\",\n          \"maxLength\": 1024,\n          \"pattern\": \"^s3://.*$\"\n        },\n        \"ContentType\": {\n          \"type\": \"string\",\n          \"description\": \"The content type of the input documents.\",\n          \"maxLength\": 256\n        }\n      }\n    },\n    \"OutputDataConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The output data configuration for the translation job.\",\n      \"required\": [\n        \"S3Uri\"\n      ],\n      \"properties\": {\n        \"S3Uri\": {\n          \"type\": \"string\",\n          \"description\": \"The URI of the S3 folder for the output documents.\",\n          \"maxLength\": 1024,\n          \"pattern\": \"^s3://.*$\"\n        }\n      }\n    },\n    \"DataAccessRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the IAM role\
  \ for S3 access.\",\n      \"pattern\": \"^arn:aws:iam::.+:role/.+\"\n    },\n    \"TerminologyNames\": {\n      \"type\": \"array\",\n      \"description\": \"The names of custom terminologies applied to the job.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"SubmittedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the translation job was submitted.\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the translation job ended.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of tags associated with the translation job.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value pair for tagging resources.\",\n      \"required\": [\n        \"Key\",\n        \"Value\"\
  \n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"minLength\": 0,\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-translate/refs/heads/main/json-schema/amazon-translate-job-schema.json
tags:
- AWS
- Language Processing
- Localization
- Machine Translation
- NLP
- Translation
title: Amazon Translate Translation Job
---
