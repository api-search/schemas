---
description: ''
layout: schema
name: S3Uri
properties_list: []
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-s3-uri-schema.json
slug: healthimaging-s3-uri
source_filename: healthimaging-s3-uri-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-s3-uri-schema.json\",\n  \"title\": \"S3Uri\",\n  \"type\": \"string\",\n  \"pattern\": \"s3://[a-z0-9][\\\\.\\\\-a-z0-9]{1,61}[a-z0-9](/.*)?\",\n  \"minLength\": 1,\n  \"maxLength\": 1024\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-s3-uri-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: S3Uri
---
