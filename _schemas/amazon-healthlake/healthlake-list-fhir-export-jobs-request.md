---
description: ''
layout: schema
name: ListFHIRExportJobsRequest
properties_list:
- description: ''
  name: DatastoreId
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobStatus
  type: object
- description: ''
  name: SubmittedBefore
  type: object
- description: ''
  name: SubmittedAfter
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-list-fhir-export-jobs-request-schema.json
slug: healthlake-list-fhir-export-jobs-request
source_filename: healthlake-list-fhir-export-jobs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-list-fhir-export-jobs-request-schema.json\",\n  \"title\": \"ListFHIRExportJobsRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastoreId\"\n  ],\n  \"properties\": {\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \" This parameter limits the response to the export job with the specified data store ID. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" A pagination token used to identify the next page of results to return for a ListFHIRExportJobs query. \"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/MaxResultsInteger\"\n        },\n        {\n          \"description\": \" This parameter limits the number of results returned for a ListFHIRExportJobs to a maximum quantity specified by the user. \"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \" This parameter limits the response to the export job with the specified job name. \"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \" This parameter limits the response to the export jobs with the specified job status. \"\n        }\n      ]\n    },\n    \"SubmittedBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\"\
  : \" This parameter limits the response to FHIR export jobs submitted before a user specified date. \"\n        }\n      ]\n    },\n    \"SubmittedAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" This parameter limits the response to FHIR export jobs submitted after a user specified date. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-list-fhir-export-jobs-request-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: ListFHIRExportJobsRequest
---
