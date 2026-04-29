---
description: ''
layout: schema
name: StartDICOMImportJobRequest
properties_list:
- description: ''
  name: jobName
  type: object
- description: ''
  name: dataAccessRoleArn
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: inputS3Uri
  type: object
- description: ''
  name: outputS3Uri
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-start-dicom-import-job-request-schema.json
slug: healthimaging-start-dicom-import-job-request
source_filename: healthimaging-start-dicom-import-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-start-dicom-import-job-request-schema.json\",\n  \"title\": \"StartDICOMImportJobRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"dataAccessRoleArn\",\n    \"clientToken\",\n    \"inputS3Uri\",\n    \"outputS3Uri\"\n  ],\n  \"properties\": {\n    \"jobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The import job name.\"\n        }\n      ]\n    },\n    \"dataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants permission to access medical imaging resources.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A unique identifier for API idempotency.\"\n        }\n      ]\n    },\n    \"inputS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The input prefix path for the S3 bucket that contains the DICOM files to be imported.\"\n        }\n      ]\n    },\n    \"outputS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The output prefix of the S3 bucket to upload the results of the DICOM import job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-start-dicom-import-job-request-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: StartDICOMImportJobRequest
---
