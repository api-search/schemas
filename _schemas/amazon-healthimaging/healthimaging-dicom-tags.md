---
description: The DICOM attributes returned as a part of a response. Each image set has these properties as part of a search result.
layout: schema
name: DICOMTags
properties_list:
- description: ''
  name: DICOMPatientId
  type: object
- description: ''
  name: DICOMPatientName
  type: object
- description: ''
  name: DICOMPatientBirthDate
  type: object
- description: ''
  name: DICOMPatientSex
  type: object
- description: ''
  name: DICOMStudyInstanceUID
  type: object
- description: ''
  name: DICOMStudyId
  type: object
- description: ''
  name: DICOMStudyDescription
  type: object
- description: ''
  name: DICOMNumberOfStudyRelatedSeries
  type: object
- description: ''
  name: DICOMNumberOfStudyRelatedInstances
  type: object
- description: ''
  name: DICOMAccessionNumber
  type: object
- description: ''
  name: DICOMStudyDate
  type: object
- description: ''
  name: DICOMStudyTime
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-dicom-tags-schema.json
slug: healthimaging-dicom-tags
source_filename: healthimaging-dicom-tags-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-dicom-tags-schema.json\",\n  \"title\": \"DICOMTags\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DICOMPatientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMPatientId\"\n        },\n        {\n          \"description\": \"The unique identifier for a patient in a DICOM Study.\"\n        }\n      ]\n    },\n    \"DICOMPatientName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMPatientName\"\n        },\n        {\n          \"description\": \"The patient name.\"\n        }\n      ]\n    },\n    \"DICOMPatientBirthDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMPatientBirthDate\"\n        },\n        {\n          \"description\": \"The patient birth date.\"\n\
  \        }\n      ]\n    },\n    \"DICOMPatientSex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMPatientSex\"\n        },\n        {\n          \"description\": \"The patient sex.\"\n        }\n      ]\n    },\n    \"DICOMStudyInstanceUID\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMStudyInstanceUID\"\n        },\n        {\n          \"description\": \"The DICOM provided identifier for studyInstanceUid.&gt;\"\n        }\n      ]\n    },\n    \"DICOMStudyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMStudyId\"\n        },\n        {\n          \"description\": \"The DICOM provided studyId.\"\n        }\n      ]\n    },\n    \"DICOMStudyDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMStudyDescription\"\n        },\n        {\n          \"description\": \"The description of the study.\"\n        }\n      ]\n    },\n    \"\
  DICOMNumberOfStudyRelatedSeries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMNumberOfStudyRelatedSeries\"\n        },\n        {\n          \"description\": \"The total number of series in the DICOM study.\"\n        }\n      ]\n    },\n    \"DICOMNumberOfStudyRelatedInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMNumberOfStudyRelatedInstances\"\n        },\n        {\n          \"description\": \"The total number of instances in the DICOM study.\"\n        }\n      ]\n    },\n    \"DICOMAccessionNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMAccessionNumber\"\n        },\n        {\n          \"description\": \"The accession number for the DICOM study.\"\n        }\n      ]\n    },\n    \"DICOMStudyDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMStudyDate\"\n        },\n        {\n          \"description\": \"The\
  \ study date.\"\n        }\n      ]\n    },\n    \"DICOMStudyTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMStudyTime\"\n        },\n        {\n          \"description\": \"The study time.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The DICOM attributes returned as a part of a response. Each image set has these properties as part of a search result.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-dicom-tags-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: DICOMTags
---
