---
description: Schema representing a CDISC SDTM or ADaM dataset domain specification including all variables.
layout: schema
name: CDISC Dataset (Domain)
properties_list:
- description: Dataset/domain abbreviation (e.g., AE, CM, DM)
  name: name
  type: string
- description: Human-readable label for the dataset
  name: label
  type: string
- description: Detailed description of the dataset purpose and content
  name: description
  type: string
- description: SDTM general observation class
  name: datasetClass
  type: string
- description: Dataset structure (one record per subject, one record per visit, etc.)
  name: structure
  type: string
- description: 'Dataset purpose: Tabulation or Analysis'
  name: purpose
  type: string
- description: Key variables that uniquely identify a record
  name: keys
  type: array
- description: List of variables (columns) in the dataset
  name: variables
  type: array
- description: HAL hypermedia links
  name: _links
  type: object
provider_name: cdisc
provider_slug: cdisc
schema_file: json-schema/cdisc-dataset-schema.json
slug: cdisc-dataset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://library.cdisc.org/api/schemas/dataset\",\n  \"title\": \"CDISC Dataset (Domain)\",\n  \"description\": \"Schema representing a CDISC SDTM or ADaM dataset domain specification including all variables.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"label\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset/domain abbreviation (e.g., AE, CM, DM)\",\n      \"pattern\": \"^[A-Z]{2,4}$\",\n      \"examples\": [\"AE\", \"CM\", \"DM\", \"EX\", \"LB\"]\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable label for the dataset\",\n      \"examples\": [\"Adverse Events\", \"Concomitant/Prior Medications\", \"Demographics\"]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the dataset purpose and content\"\n    },\n    \"datasetClass\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"SDTM general observation class\",\n      \"enum\": [\"Events\", \"Findings\", \"Interventions\", \"Special Purpose\", \"Relationship\", \"Trial Design\"]\n    },\n    \"structure\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset structure (one record per subject, one record per visit, etc.)\"\n    },\n    \"purpose\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset purpose: Tabulation or Analysis\",\n      \"enum\": [\"Tabulation\", \"Analysis\"]\n    },\n    \"keys\": {\n      \"type\": \"array\",\n      \"description\": \"Key variables that uniquely identify a record\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [[\"STUDYID\", \"USUBJID\", \"AESEQ\"]]\n    },\n    \"variables\": {\n      \"type\": \"array\",\n      \"description\": \"List of variables (columns) in the dataset\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Variable\"\n      }\n    },\n\
  \    \"_links\": {\n      \"type\": \"object\",\n      \"description\": \"HAL hypermedia links\",\n      \"properties\": {\n        \"self\": {\n          \"$ref\": \"#/$defs/Link\"\n        },\n        \"parentClass\": {\n          \"$ref\": \"#/$defs/Link\"\n        },\n        \"parentProduct\": {\n          \"$ref\": \"#/$defs/Link\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"Variable\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"label\", \"dataType\", \"core\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Variable name (e.g., AETERM)\",\n          \"pattern\": \"^[A-Z][A-Z0-9]{1,7}$\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"Variable label (40 char max)\",\n          \"maxLength\": 40\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Detailed variable description\"\n        },\n\
  \        \"dataType\": {\n          \"type\": \"string\",\n          \"description\": \"SAS data type\",\n          \"enum\": [\"Char\", \"Num\", \"date\", \"datetime\", \"partialDate\", \"partialDatetime\", \"time\", \"partialTime\", \"integer\", \"float\", \"text\", \"uri\"]\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum length for character variables\",\n          \"minimum\": 1\n        },\n        \"significantDigits\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of significant digits for numeric variables\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"description\": \"SAS format for display\",\n          \"examples\": [\"DATE9.\", \"TIME5.\", \"DATETIME19.\"]\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"description\": \"Variable role within the SDTM general observation class\",\n          \"enum\": [\n            \"Identifier\"\
  ,\n            \"Topic\",\n            \"Record Qualifier\",\n            \"Result Qualifier\",\n            \"Synonym Qualifier\",\n            \"Variable Qualifier\",\n            \"Timing\",\n            \"Rule\",\n            \"Grouping Qualifier\"\n          ]\n        },\n        \"core\": {\n          \"type\": \"string\",\n          \"description\": \"Variable core status indicating requirement level\",\n          \"enum\": [\"Required\", \"Expected\", \"Permissible\", \"Conditionally Required\", \"Conditionally Expected\"]\n        },\n        \"codelistSubmissionValues\": {\n          \"type\": \"array\",\n          \"description\": \"Applicable CDISC controlled terminology codelist submission values\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"valueList\": {\n          \"type\": \"array\",\n          \"description\": \"Enumerated list of allowed values\",\n          \"items\": {\n            \"type\": \"string\"\n         \
  \ }\n        },\n        \"ordinal\": {\n          \"type\": \"integer\",\n          \"description\": \"Variable ordering position within the dataset\"\n        },\n        \"simpleDatatype\": {\n          \"type\": \"string\",\n          \"description\": \"Simplified datatype\",\n          \"enum\": [\"text\", \"integer\", \"float\", \"date\", \"datetime\", \"time\"]\n        }\n      }\n    },\n    \"Link\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"title\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/json-schema/cdisc-dataset-schema.json
tags: []
title: CDISC Dataset (Domain)
---
