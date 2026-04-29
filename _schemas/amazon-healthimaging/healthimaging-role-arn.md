---
description: ''
layout: schema
name: RoleArn
properties_list: []
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-role-arn-schema.json
slug: healthimaging-role-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-role-arn-schema.json\",\n  \"title\": \"RoleArn\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws(-[^:]+)?:iam::[0-9]{12}:role/.+\",\n  \"minLength\": 20,\n  \"maxLength\": 2048\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-role-arn-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: RoleArn
---
