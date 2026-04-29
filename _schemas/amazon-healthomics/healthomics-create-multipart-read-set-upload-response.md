---
description: ''
layout: schema
name: CreateMultipartReadSetUploadResponse
properties_list:
- description: ''
  name: sequenceStoreId
  type: object
- description: ''
  name: uploadId
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
- description: ''
  name: creationTime
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-create-multipart-read-set-upload-response-schema.json
slug: healthomics-create-multipart-read-set-upload-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-multipart-read-set-upload-response-schema.json\",\n  \"title\": \"CreateMultipartReadSetUploadResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"sequenceStoreId\",\n    \"uploadId\",\n    \"sourceFileType\",\n    \"subjectId\",\n    \"sampleId\",\n    \"referenceArn\",\n    \"creationTime\"\n  ],\n  \"properties\": {\n    \"sequenceStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreId\"\n        },\n        {\n          \"description\": \" The sequence store ID for the store that the read set will be created in. \"\n        }\n      ]\n    },\n    \"uploadId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UploadId\"\n        },\n        {\n          \"description\": \" he ID for the initiated\
  \ multipart upload. \"\n        }\n      ]\n    },\n    \"sourceFileType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileType\"\n        },\n        {\n          \"description\": \" The file type of the read set source. \"\n        }\n      ]\n    },\n    \"subjectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubjectId\"\n        },\n        {\n          \"description\": \" The source's subject ID. \"\n        }\n      ]\n    },\n    \"sampleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleId\"\n        },\n        {\n          \"description\": \" The source's sample ID. \"\n        }\n      ]\n    },\n    \"generatedFrom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneratedFrom\"\n        },\n        {\n          \"description\": \" The source of the read set. \"\n        }\n      ]\n    },\n    \"referenceArn\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/ReferenceArn\"\n        },\n        {\n          \"description\": \" The read set source's reference ARN. \"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetName\"\n        },\n        {\n          \"description\": \" The name of the read set. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetDescription\"\n        },\n        {\n          \"description\": \" The description of the read set. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \" The tags to add to the read set. \"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n  \
  \      },\n        {\n          \"description\": \" The creation time of the multipart upload. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-multipart-read-set-upload-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CreateMultipartReadSetUploadResponse
---
