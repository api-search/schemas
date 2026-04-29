---
description: ''
layout: schema
name: BoundedLengthString
properties_list: []
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-bounded-length-string-schema.json
slug: healthlake-bounded-length-string
source_filename: healthlake-bounded-length-string-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-bounded-length-string-schema.json\",\n  \"title\": \"BoundedLengthString\",\n  \"type\": \"string\",\n  \"pattern\": \"[\\\\P{M}\\\\p{M}]{1,5000}\",\n  \"minLength\": 1,\n  \"maxLength\": 5000\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-bounded-length-string-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: BoundedLengthString
---
