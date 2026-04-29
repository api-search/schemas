---
description: ''
layout: schema
name: IamRoleArn
properties_list: []
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-iam-role-arn-schema.json
slug: healthlake-iam-role-arn
source_filename: healthlake-iam-role-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-iam-role-arn-schema.json\",\n  \"title\": \"IamRoleArn\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws(-[^:]+)?:iam::[0-9]{12}:role/.+\",\n  \"minLength\": 20,\n  \"maxLength\": 2048\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-iam-role-arn-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: IamRoleArn
---
