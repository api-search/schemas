---
description: A source for an import read set job.
layout: schema
name: ImportReadSetSourceItem
properties_list:
- description: ''
  name: sourceFiles
  type: object
- description: ''
  name: sourceFileType
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusMessage
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
schema_file: json-schema/healthomics-import-read-set-source-item-schema.json
slug: healthomics-import-read-set-source-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-import-read-set-source-item-schema.json\",\n  \"title\": \"ImportReadSetSourceItem\",\n  \"type\": \"object\",\n  \"required\": [\n    \"sourceFiles\",\n    \"sourceFileType\",\n    \"status\",\n    \"subjectId\",\n    \"sampleId\"\n  ],\n  \"properties\": {\n    \"sourceFiles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceFiles\"\n        },\n        {\n          \"description\": \"The source files' location in Amazon S3.\"\n        }\n      ]\n    },\n    \"sourceFileType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileType\"\n        },\n        {\n          \"description\": \"The source's file type.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetImportJobItemStatus\"\
  \n        },\n        {\n          \"description\": \"The source's status.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatusMessage\"\n        },\n        {\n          \"description\": \"The source's status message.\"\n        }\n      ]\n    },\n    \"subjectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubjectId\"\n        },\n        {\n          \"description\": \"The source's subject ID.\"\n        }\n      ]\n    },\n    \"sampleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleId\"\n        },\n        {\n          \"description\": \"The source's sample ID.\"\n        }\n      ]\n    },\n    \"generatedFrom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneratedFrom\"\n        },\n        {\n          \"description\": \"Where the source originated.\"\n        }\n      ]\n    },\n \
  \   \"referenceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceArn\"\n        },\n        {\n          \"description\": \"The source's genome reference ARN.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetName\"\n        },\n        {\n          \"description\": \"The source's name.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetDescription\"\n        },\n        {\n          \"description\": \"The source's description.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The source's tags.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A source for an import read set job.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-import-read-set-source-item-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ImportReadSetSourceItem
---
