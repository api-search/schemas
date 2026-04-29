---
description: ''
layout: schema
name: TagKey
properties_list: []
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-tag-key-schema.json
slug: healthimaging-tag-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-tag-key-schema.json\",\n  \"title\": \"TagKey\",\n  \"type\": \"string\",\n  \"pattern\": \"(?!aws:)[a-zA-Z+-=._:/]+\",\n  \"minLength\": 1,\n  \"maxLength\": 128\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-tag-key-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: TagKey
---
