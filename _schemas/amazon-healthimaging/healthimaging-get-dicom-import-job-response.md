---
description: ''
layout: schema
name: GetDICOMImportJobResponse
properties_list:
- description: ''
  name: jobProperties
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-get-dicom-import-job-response-schema.json
slug: healthimaging-get-dicom-import-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-get-dicom-import-job-response-schema.json\",\n  \"title\": \"GetDICOMImportJobResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"jobProperties\"\n  ],\n  \"properties\": {\n    \"jobProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMImportJobProperties\"\n        },\n        {\n          \"description\": \"The properties of the import job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-get-dicom-import-job-response-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: GetDICOMImportJobResponse
---
