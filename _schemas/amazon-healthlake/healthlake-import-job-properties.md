---
description: Displays the properties of the import job, including the ID, Arn, Name, and the status of the data store.
layout: schema
name: ImportJobProperties
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobStatus
  type: object
- description: ''
  name: SubmitTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: DatastoreId
  type: object
- description: ''
  name: InputDataConfig
  type: object
- description: ''
  name: JobOutputDataConfig
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-import-job-properties-schema.json
slug: healthlake-import-job-properties
source_filename: healthlake-import-job-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-import-job-properties-schema.json\",\n  \"title\": \"ImportJobProperties\",\n  \"type\": \"object\",\n  \"required\": [\n    \"JobId\",\n    \"JobStatus\",\n    \"SubmitTime\",\n    \"DatastoreId\",\n    \"InputDataConfig\"\n  ],\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The AWS-generated id number for the Import job.\"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The user-generated name for an Import job.\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\
  \n        },\n        {\n          \"description\": \"The job status for an Import job. Possible statuses are SUBMITTED, IN_PROGRESS, COMPLETED_WITH_ERRORS, COMPLETED, FAILED.\"\n        }\n      ]\n    },\n    \"SubmitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the Import job was submitted for processing.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the Import job was completed.\"\n        }\n      ]\n    },\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The datastore id used when the Import job was created. \"\n        }\n      ]\n    },\n    \"InputDataConfig\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/InputDataConfig\"\n        },\n        {\n          \"description\": \"The input data configuration that was supplied when the Import job was created.\"\n        }\n      ]\n    },\n    \"JobOutputDataConfig\": {\n      \"$ref\": \"#/components/schemas/OutputDataConfig\"\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that gives AWS HealthLake access to your input data.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"An explanation of any errors that may have occurred during the FHIR import job. \"\n        }\n      ]\n    }\n  },\n  \"description\": \"Displays the properties of the import job, including the ID, Arn, Name, and the status of\
  \ the data store.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-import-job-properties-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: ImportJobProperties
---
