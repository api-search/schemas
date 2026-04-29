---
description: ''
layout: schema
name: S3Uri
properties_list: []
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-s3-uri-schema.json
slug: healthlake-s3-uri
source_filename: healthlake-s3-uri-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-s3-uri-schema.json\",\n  \"title\": \"S3Uri\",\n  \"type\": \"string\",\n  \"pattern\": \"s3://[a-z0-9][\\\\.\\\\-a-z0-9]{1,61}[a-z0-9](/.*)?\",\n  \"maxLength\": 1024\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-s3-uri-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: S3Uri
---
