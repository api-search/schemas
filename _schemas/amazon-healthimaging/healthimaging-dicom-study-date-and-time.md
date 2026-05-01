---
description: The aggregated structure to store DICOM study date and study time for search capabilities.
layout: schema
name: DICOMStudyDateAndTime
properties_list:
- description: ''
  name: DICOMStudyDate
  type: object
- description: ''
  name: DICOMStudyTime
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-dicom-study-date-and-time-schema.json
slug: healthimaging-dicom-study-date-and-time
source_filename: healthimaging-dicom-study-date-and-time-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-dicom-study-date-and-time-schema.json\",\n  \"title\": \"DICOMStudyDateAndTime\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DICOMStudyDate\"\n  ],\n  \"properties\": {\n    \"DICOMStudyDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMStudyDate\"\n        },\n        {\n          \"description\": \"The DICOM study date provided in <code>yyMMdd</code> format.\"\n        }\n      ]\n    },\n    \"DICOMStudyTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMStudyTime\"\n        },\n        {\n          \"description\": \"The DICOM study time provided in <code>HHmmss.FFFFFF</code> format.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The aggregated structure to store DICOM study date and study\
  \ time for search capabilities.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-dicom-study-date-and-time-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: DICOMStudyDateAndTime
---
