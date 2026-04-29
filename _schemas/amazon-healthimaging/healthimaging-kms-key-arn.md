---
description: ARN referencing a KMS key or KMS key alias.
layout: schema
name: KmsKeyArn
properties_list: []
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-kms-key-arn-schema.json
slug: healthimaging-kms-key-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-kms-key-arn-schema.json\",\n  \"title\": \"KmsKeyArn\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws[a-zA-Z-]{0,16}:kms:[a-z]{2}(-[a-z]{1,16}){1,3}-\\\\d{1}:\\\\d{12}:((key/[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12})|(alias/[a-zA-Z0-9:/_-]{1,256}))\",\n  \"description\": \"ARN referencing a KMS key or KMS key alias.\",\n  \"minLength\": 1,\n  \"maxLength\": 512\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-kms-key-arn-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: KmsKeyArn
---
