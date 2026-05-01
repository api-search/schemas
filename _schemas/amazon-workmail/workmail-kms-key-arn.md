---
description: KmsKeyArn schema from Amazon WorkMail API
layout: schema
name: KmsKeyArn
properties_list: []
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-kms-key-arn-schema.json
slug: workmail-kms-key-arn
source_filename: workmail-kms-key-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws:kms:[a-z0-9-]*:[a-z0-9-]+:[A-Za-z0-9][A-Za-z0-9:_/+=,@.-]{0,1023}\",\n  \"minLength\": 20,\n  \"maxLength\": 2048,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KmsKeyArn\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-kms-key-arn-schema.json\",\n  \"description\": \"KmsKeyArn schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-kms-key-arn-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: KmsKeyArn
---
