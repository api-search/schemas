---
description: ''
layout: schema
name: ListDICOMImportJobsResponse
properties_list:
- description: ''
  name: jobSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-list-dicom-import-jobs-response-schema.json
slug: healthimaging-list-dicom-import-jobs-response
source_filename: healthimaging-list-dicom-import-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-list-dicom-import-jobs-response-schema.json\",\n  \"title\": \"ListDICOMImportJobsResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"jobSummaries\"\n  ],\n  \"properties\": {\n    \"jobSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMImportJobSummaries\"\n        },\n        {\n          \"description\": \"A list of job summaries.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token used to retrieve the list of import jobs on the next page.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-list-dicom-import-jobs-response-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: ListDICOMImportJobsResponse
---
