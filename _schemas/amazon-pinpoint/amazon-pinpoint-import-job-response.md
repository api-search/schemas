---
description: Provides information about the status and settings of a job that imports endpoint definitions from one or more files. The files can be stored in an Amazon Simple Storage Service (Amazon S3) bucket or uploaded directly from a computer by using the Amazon Pinpoint console.
layout: schema
name: ImportJobResponse
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: CompletedPieces
  type: object
- description: ''
  name: CompletionDate
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Definition
  type: object
- description: ''
  name: FailedPieces
  type: object
- description: ''
  name: Failures
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: JobStatus
  type: object
- description: ''
  name: TotalFailures
  type: object
- description: ''
  name: TotalPieces
  type: object
- description: ''
  name: TotalProcessed
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-import-job-response-schema.json
slug: amazon-pinpoint-import-job-response
source_filename: amazon-pinpoint-import-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-import-job-response-schema.json\",\n  \"title\": \"ImportJobResponse\",\n  \"description\": \"Provides information about the status and settings of a job that imports endpoint definitions from one or more files. The files can be stored in an Amazon Simple Storage Service (Amazon S3) bucket or uploaded directly from a computer by using the Amazon Pinpoint console.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that's associated with the import job.\"\n        }\n      ]\n    },\n    \"CompletedPieces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\
  \n        },\n        {\n          \"description\": \"The number of pieces that were processed successfully (completed) by the import job, as of the time of the request.\"\n        }\n      ]\n    },\n    \"CompletionDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the import job was completed.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the import job was created.\"\n        }\n      ]\n    },\n    \"Definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportJobResource\"\n        },\n        {\n          \"description\": \"The resource settings that apply to the import job.\"\n        }\n      ]\n    },\n    \"FailedPieces\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The number of pieces that weren't processed successfully (failed) by the import job, as of the time of the request.\"\n        }\n      ]\n    },\n    \"Failures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOf__string\"\n        },\n        {\n          \"description\": \"An array of entries, one for each of the first 100 entries that weren't processed successfully (failed) by the import job, if any.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the import job.\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"\
  The status of the import job. The job status is FAILED if Amazon Pinpoint wasn't able to process one or more pieces in the job.\"\n        }\n      ]\n    },\n    \"TotalFailures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The total number of endpoint definitions that weren't processed successfully (failed) by the import job, typically because an error, such as a syntax error, occurred.\"\n        }\n      ]\n    },\n    \"TotalPieces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The total number of pieces that must be processed to complete the import job. Each piece consists of an approximately equal portion of the endpoint definitions that are part of the import job.\"\n        }\n      ]\n    },\n    \"TotalProcessed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\
  \n        },\n        {\n          \"description\": \"The total number of endpoint definitions that were processed by the import job.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The job type. This value is IMPORT for import jobs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobStatus\",\n    \"CreationDate\",\n    \"Type\",\n    \"Definition\",\n    \"Id\",\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-import-job-response-schema.json
tags:
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: ImportJobResponse
---
