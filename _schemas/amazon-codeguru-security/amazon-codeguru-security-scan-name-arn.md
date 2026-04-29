---
description: ScanNameArn schema from Amazon CodeGuru Security
layout: schema
name: ScanNameArn
properties_list: []
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-scan-name-arn-schema.json
slug: amazon-codeguru-security-scan-name-arn
source_filename: amazon-codeguru-security-scan-name-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-scan-name-arn-schema.json\",\n  \"title\": \"ScanNameArn\",\n  \"description\": \"ScanNameArn schema from Amazon CodeGuru Security\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws:codeguru-security:[\\\\S]+:[\\\\d]{12}:scans\\\\/[a-zA-Z0-9-_$:.]*$\",\n  \"minLength\": 1,\n  \"maxLength\": 300\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-scan-name-arn-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: ScanNameArn
---
