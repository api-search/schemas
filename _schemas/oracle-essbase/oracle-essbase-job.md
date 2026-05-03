---
description: An asynchronous job executed on an Essbase database. Jobs support operations such as data loading, dimension building, calculations, data clearing, Excel import/export, LCM backup/restore, aggregation management, ASO buffer operations, data export, and MDX script execution.
layout: schema
name: Oracle Essbase Job
properties_list:
- description: Unique job identifier assigned by the server.
  name: job_ID
  type: integer
- description: Name of the application the job was executed against.
  name: appName
  type: string
- description: Name of the database the job was executed against.
  name: dbName
  type: string
- description: Type of job that was executed.
  name: jobType
  type: string
- description: Name of the script or file associated with the job.
  name: jobfileName
  type: string
- description: User ID of the person who submitted the job.
  name: userName
  type: string
- description: Job start time in milliseconds since Unix epoch.
  name: startTime
  type: integer
- description: Job end time in milliseconds since Unix epoch. Null if the job is still running.
  name: endTime
  type: integer
- description: Numeric status code indicating job state. 100=In Progress, 200=Completed, 300=Completed with Warnings, 400=Failed.
  name: statusCode
  type: integer
- description: Human-readable status message describing the current job state.
  name: statusMessage
  type: string
- description: Input parameters that were used to execute the job. Structure varies by job type.
  name: jobInputInfo
  type: object
- description: Output and results of the job execution. Structure varies by job type.
  name: jobOutputInfo
  type: object
- description: HATEOAS navigation links.
  name: links
  type: array
provider_name: Oracle Essbase
provider_slug: oracle-essbase
schema_file: json-schema/oracle-essbase-job-schema.json
slug: oracle-essbase-job
source_filename: oracle-essbase-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"oracle-essbase-job-schema.json\",\n  \"title\": \"Oracle Essbase Job\",\n  \"description\": \"An asynchronous job executed on an Essbase database. Jobs support operations such as data loading, dimension building, calculations, data clearing, Excel import/export, LCM backup/restore, aggregation management, ASO buffer operations, data export, and MDX script execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job_ID\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique job identifier assigned by the server.\"\n    },\n    \"appName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the application the job was executed against.\"\n    },\n    \"dbName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the database the job was executed against.\"\n    },\n    \"jobType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of\
  \ job that was executed.\"\n    },\n    \"jobfileName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the script or file associated with the job.\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the person who submitted the job.\"\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Job start time in milliseconds since Unix epoch.\"\n    },\n    \"endTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Job end time in milliseconds since Unix epoch. Null if the job is still running.\"\n    },\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric status code indicating job state. 100=In Progress, 200=Completed, 300=Completed with Warnings, 400=Failed.\",\n      \"enum\": [100, 200, 300, 400]\n    },\n    \"statusMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable status message describing the current job state.\"\
  \n    },\n    \"jobInputInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters that were used to execute the job. Structure varies by job type.\",\n      \"additionalProperties\": true\n    },\n    \"jobOutputInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Output and results of the job execution. Structure varies by job type.\",\n      \"additionalProperties\": true,\n      \"properties\": {\n        \"recordsProcessed\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of records successfully processed (for data load jobs).\"\n        },\n        \"recordsRejected\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of records rejected during processing (for data load jobs).\"\n        },\n        \"errorMessage\": {\n          \"type\": \"string\",\n          \"description\": \"Error message if the job failed or had warnings.\"\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"HATEOAS navigation links.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Link\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"JobInput\": {\n      \"type\": \"object\",\n      \"description\": \"Input for executing an asynchronous job.\",\n      \"required\": [\"jobtype\"],\n      \"properties\": {\n        \"application\": {\n          \"type\": \"string\",\n          \"description\": \"Application name.\"\n        },\n        \"db\": {\n          \"type\": \"string\",\n          \"description\": \"Database name.\"\n        },\n        \"jobtype\": {\n          \"type\": \"string\",\n          \"description\": \"Type of job to execute.\",\n          \"enum\": [\n            \"dataload\",\n            \"dimbuild\",\n            \"calc\",\n            \"clear\",\n            \"importExcel\",\n            \"exportExcel\",\n            \"lcmExport\",\n            \"lcmImport\",\n            \"clearAggregation\",\n            \"buildAggregation\",\n        \
  \    \"asoBufferDataLoad\",\n            \"asoBufferCommit\",\n            \"exportData\",\n            \"mdxScript\"\n          ]\n        },\n        \"parameters\": {\n          \"$ref\": \"#/$defs/JobParameters\"\n        }\n      }\n    },\n    \"JobParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Job-specific parameters. Required fields depend on the job type.\",\n      \"properties\": {\n        \"file\": {\n          \"type\": \"string\",\n          \"description\": \"Source file name for dataload, dimbuild, or mdxScript jobs.\"\n        },\n        \"rule\": {\n          \"type\": \"string\",\n          \"description\": \"Rules file name for dataload or dimbuild jobs.\"\n        },\n        \"abortOnError\": {\n          \"type\": \"string\",\n          \"description\": \"Stop on first error (true/false) for dataload jobs.\"\n        },\n        \"script\": {\n          \"type\": \"string\",\n          \"description\": \"Calculation script name (.csc file)\
  \ for calc jobs.\"\n        },\n        \"option\": {\n          \"type\": \"string\",\n          \"description\": \"Clear option for clear jobs.\",\n          \"enum\": [\"allData\", \"upperLevel\", \"nonInput\", \"partialData\", \"PARTIAL_DATA\"]\n        },\n        \"partialDataExpression\": {\n          \"type\": \"string\",\n          \"description\": \"MDX expression for partial data clear.\"\n        },\n        \"zipFileName\": {\n          \"type\": \"string\",\n          \"description\": \"Backup zip file name for lcmExport/lcmImport jobs.\"\n        },\n        \"dataLevel\": {\n          \"type\": \"string\",\n          \"description\": \"Data level for export operations.\",\n          \"enum\": [\"ALL_DATA\", \"UPPER_LEVEL_BLOCKS\", \"NON_INPUT_BLOCKS\", \"LEVEL_ZERO_BLOCKS\", \"INPUT_LEVEL_DATA_BLOCKS\"]\n        },\n        \"restructureOption\": {\n          \"type\": \"string\",\n          \"description\": \"Data preservation option for dimension build jobs.\",\n    \
  \      \"enum\": [\"PRESERVE_ALL_DATA\", \"PRESERVE_NO_DATA\", \"PRESERVE_LEAFLEVEL_DATA\", \"PRESERVE_INPUT_DATA\"]\n        },\n        \"commitOption\": {\n          \"type\": \"string\",\n          \"description\": \"Commit option for ASO buffer commit jobs.\",\n          \"enum\": [\"STORE_DATA\", \"ADD_DATA\", \"SUBTRACT_DATA\", \"OVERRIDE_ALL_DATA\", \"OVERRIDE_INCREMENTAL_DATA\"]\n        }\n      }\n    },\n    \"Link\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS navigation link.\",\n      \"properties\": {\n        \"rel\": {\n          \"type\": \"string\",\n          \"description\": \"Link relation type.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Link URL.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method for this link.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Media type of the linked resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/json-schema/oracle-essbase-job-schema.json
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
title: Oracle Essbase Job
---
