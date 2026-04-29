---
description: KmsKeyArn schema from Amazon CodeGuru Security
layout: schema
name: KmsKeyArn
properties_list: []
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-kms-key-arn-schema.json
slug: amazon-codeguru-security-kms-key-arn
source_filename: amazon-codeguru-security-kms-key-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-kms-key-arn-schema.json\",\n  \"title\": \"KmsKeyArn\",\n  \"description\": \"KmsKeyArn schema from Amazon CodeGuru Security\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws:kms:[\\\\S]+:[\\\\d]{12}:key\\\\/(([a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12})|(mrk-[0-9a-zA-Z]{32}))$\",\n  \"minLength\": 1,\n  \"maxLength\": 2048\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-kms-key-arn-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: KmsKeyArn
---
