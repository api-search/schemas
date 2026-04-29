---
description: A filter for read sets.
layout: schema
name: ReadSetFilter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: referenceArn
  type: object
- description: ''
  name: createdAfter
  type: object
- description: ''
  name: createdBefore
  type: object
- description: ''
  name: sampleId
  type: object
- description: ''
  name: subjectId
  type: object
- description: ''
  name: generatedFrom
  type: object
- description: ''
  name: creationType
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-read-set-filter-schema.json
slug: healthomics-read-set-filter
source_filename: healthomics-read-set-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-set-filter-schema.json\",\n  \"title\": \"ReadSetFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetName\"\n        },\n        {\n          \"description\": \"A name to filter on.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetStatus\"\n        },\n        {\n          \"description\": \"A status to filter on.\"\n        }\n      ]\n    },\n    \"referenceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceArn\"\n        },\n        {\n          \"description\": \"A genome reference ARN to filter on.\"\n        }\n      ]\n    },\n    \"createdAfter\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The filter's start date.\"\n        }\n      ]\n    },\n    \"createdBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The filter's end date.\"\n        }\n      ]\n    },\n    \"sampleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleId\"\n        },\n        {\n          \"description\": \" The read set source's sample ID. \"\n        }\n      ]\n    },\n    \"subjectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubjectId\"\n        },\n        {\n          \"description\": \" The read set source's subject ID. \"\n        }\n      ]\n    },\n    \"generatedFrom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneratedFrom\"\
  \n        },\n        {\n          \"description\": \" Where the source originated. \"\n        }\n      ]\n    },\n    \"creationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreationType\"\n        },\n        {\n          \"description\": \" The creation type of the read set. \"\n        }\n      ]\n    }\n  },\n  \"description\": \"A filter for read sets.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-set-filter-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ReadSetFilter
---
