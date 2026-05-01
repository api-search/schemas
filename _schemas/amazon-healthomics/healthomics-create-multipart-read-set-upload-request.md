---
description: ''
layout: schema
name: CreateMultipartReadSetUploadRequest
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: sourceFileType
  type: object
- description: ''
  name: subjectId
  type: object
- description: ''
  name: sampleId
  type: object
- description: ''
  name: generatedFrom
  type: object
- description: ''
  name: referenceArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-create-multipart-read-set-upload-request-schema.json
slug: healthomics-create-multipart-read-set-upload-request
source_filename: healthomics-create-multipart-read-set-upload-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-multipart-read-set-upload-request-schema.json\",\n  \"title\": \"CreateMultipartReadSetUploadRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"sourceFileType\",\n    \"subjectId\",\n    \"sampleId\",\n    \"referenceArn\",\n    \"name\"\n  ],\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \" An idempotency token that can be used to avoid triggering multiple multipart uploads. \"\n        }\n      ]\n    },\n    \"sourceFileType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileType\"\n        },\n        {\n          \"description\": \" The type of file being uploaded. \"\n        }\n      ]\n    },\n\
  \    \"subjectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubjectId\"\n        },\n        {\n          \"description\": \" The source's subject ID. \"\n        }\n      ]\n    },\n    \"sampleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleId\"\n        },\n        {\n          \"description\": \" The source's sample ID. \"\n        }\n      ]\n    },\n    \"generatedFrom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneratedFrom\"\n        },\n        {\n          \"description\": \" Where the source originated. \"\n        }\n      ]\n    },\n    \"referenceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceArn\"\n        },\n        {\n          \"description\": \" The ARN of the reference. \"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetName\"\n\
  \        },\n        {\n          \"description\": \" The name of the read set. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetDescription\"\n        },\n        {\n          \"description\": \" The description of the read set. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \" Any tags to add to the read set. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-multipart-read-set-upload-request-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CreateMultipartReadSetUploadRequest
---
