---
description: A read set.
layout: schema
name: ReadSetListItem
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: sequenceStoreId
  type: object
- description: ''
  name: subjectId
  type: object
- description: ''
  name: sampleId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: referenceArn
  type: object
- description: ''
  name: fileType
  type: object
- description: ''
  name: sequenceInformation
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: statusMessage
  type: object
- description: ''
  name: creationType
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-read-set-list-item-schema.json
slug: healthomics-read-set-list-item
source_filename: healthomics-read-set-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-set-list-item-schema.json\",\n  \"title\": \"ReadSetListItem\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"arn\",\n    \"sequenceStoreId\",\n    \"status\",\n    \"fileType\",\n    \"creationTime\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetId\"\n        },\n        {\n          \"description\": \"The read set's ID.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetArn\"\n        },\n        {\n          \"description\": \"The read set's ARN.\"\n        }\n      ]\n    },\n    \"sequenceStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreId\"\n        },\n \
  \       {\n          \"description\": \"The read set's sequence store ID.\"\n        }\n      ]\n    },\n    \"subjectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubjectId\"\n        },\n        {\n          \"description\": \"The read set's subject ID.\"\n        }\n      ]\n    },\n    \"sampleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleId\"\n        },\n        {\n          \"description\": \"The read set's sample ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetStatus\"\n        },\n        {\n          \"description\": \"The read set's status.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetName\"\n        },\n        {\n          \"description\": \"The read set's name.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetDescription\"\n        },\n        {\n          \"description\": \"The read set's description.\"\n        }\n      ]\n    },\n    \"referenceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceArn\"\n        },\n        {\n          \"description\": \"The read set's genome reference ARN.\"\n        }\n      ]\n    },\n    \"fileType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileType\"\n        },\n        {\n          \"description\": \"The read set's file type.\"\n        }\n      ]\n    },\n    \"sequenceInformation\": {\n      \"$ref\": \"#/components/schemas/SequenceInformation\"\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"When the read set was created.\"\n        }\n      ]\n    },\n    \"statusMessage\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetStatusMessage\"\n        },\n        {\n          \"description\": \" The status for a read set. It provides more detail as to why the read set has a status. \"\n        }\n      ]\n    },\n    \"creationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreationType\"\n        },\n        {\n          \"description\": \" The creation type of the read set. \"\n        }\n      ]\n    }\n  },\n  \"description\": \"A read set.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-set-list-item-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ReadSetListItem
---
