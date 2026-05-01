---
description: The object containing <code>removableAttributes</code> and <code>updatableAttributes</code>.
layout: schema
name: DICOMUpdates
properties_list:
- description: ''
  name: removableAttributes
  type: object
- description: ''
  name: updatableAttributes
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-dicom-updates-schema.json
slug: healthimaging-dicom-updates
source_filename: healthimaging-dicom-updates-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-dicom-updates-schema.json\",\n  \"title\": \"DICOMUpdates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"removableAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMAttribute\"\n        },\n        {\n          \"description\": \"The DICOM tags to be removed from <code>ImageSetMetadata</code>.\"\n        }\n      ]\n    },\n    \"updatableAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMAttribute\"\n        },\n        {\n          \"description\": \"The DICOM tags that need to be updated in <code>ImageSetMetadata</code>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The object containing <code>removableAttributes</code> and <code>updatableAttributes</code>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-dicom-updates-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: DICOMUpdates
---
