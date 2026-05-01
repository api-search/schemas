---
description: ''
layout: schema
name: AmazonResourceName
properties_list: []
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-amazon-resource-name-schema.json
slug: healthlake-amazon-resource-name
source_filename: healthlake-amazon-resource-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-amazon-resource-name-schema.json\",\n  \"title\": \"AmazonResourceName\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws((-us-gov)|(-iso)|(-iso-b)|(-cn))?:healthlake:[a-z0-9-]+:\\\\d{12}:datastore\\\\/fhir\\\\/.{32}\",\n  \"minLength\": 1,\n  \"maxLength\": 1011\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-amazon-resource-name-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: AmazonResourceName
---
