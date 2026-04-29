---
description: The search input attribute value.
layout: schema
name: SearchByAttributeValue
properties_list:
- description: ''
  name: DICOMPatientId
  type: object
- description: ''
  name: DICOMAccessionNumber
  type: object
- description: ''
  name: DICOMStudyId
  type: object
- description: ''
  name: DICOMStudyInstanceUID
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: DICOMStudyDateAndTime
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-search-by-attribute-value-schema.json
slug: healthimaging-search-by-attribute-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-search-by-attribute-value-schema.json\",\n  \"title\": \"SearchByAttributeValue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DICOMPatientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMPatientId\"\n        },\n        {\n          \"description\": \"The patient ID input for search.\"\n        }\n      ]\n    },\n    \"DICOMAccessionNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMAccessionNumber\"\n        },\n        {\n          \"description\": \"The DICOM accession number for search.\"\n        }\n      ]\n    },\n    \"DICOMStudyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMStudyId\"\n        },\n        {\n          \"description\": \"The DICOM\
  \ study ID for search.\"\n        }\n      ]\n    },\n    \"DICOMStudyInstanceUID\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMStudyInstanceUID\"\n        },\n        {\n          \"description\": \"The DICOM study instance UID for search.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The created at time of the image set provided for search.\"\n        }\n      ]\n    },\n    \"DICOMStudyDateAndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMStudyDateAndTime\"\n        },\n        {\n          \"description\": \"The aggregated structure containing DICOM study date and study time for search.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The search input attribute value.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-search-by-attribute-value-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: SearchByAttributeValue
---
