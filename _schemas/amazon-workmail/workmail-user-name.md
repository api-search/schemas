---
description: UserName schema from Amazon WorkMail API
layout: schema
name: UserName
properties_list: []
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-user-name-schema.json
slug: workmail-user-name
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"[\\\\w\\\\-.]+(@[a-zA-Z0-9.\\\\-]+\\\\.[a-zA-Z0-9-]{2,})?\",\n  \"minLength\": 1,\n  \"maxLength\": 64,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserName\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-user-name-schema.json\",\n  \"description\": \"UserName schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-user-name-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: UserName
---
