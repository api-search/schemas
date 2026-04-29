---
description: Contains DICOMUpdates.
layout: schema
name: MetadataUpdates
properties_list:
- description: ''
  name: DICOMUpdates
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-metadata-updates-schema.json
slug: healthimaging-metadata-updates
source_filename: healthimaging-metadata-updates-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-metadata-updates-schema.json\",\n  \"title\": \"MetadataUpdates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DICOMUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMUpdates\"\n        },\n        {\n          \"description\": \"The object containing <code>removableAttributes</code> and <code>updatableAttributes</code>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains DICOMUpdates.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-metadata-updates-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: MetadataUpdates
---
