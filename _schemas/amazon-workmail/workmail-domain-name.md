---
description: DomainName schema from Amazon WorkMail API
layout: schema
name: DomainName
properties_list: []
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-domain-name-schema.json
slug: workmail-domain-name
source_filename: workmail-domain-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"[a-zA-Z0-9.-]+\\\\.[a-zA-Z-]{2,}\",\n  \"minLength\": 3,\n  \"maxLength\": 255,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DomainName\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-domain-name-schema.json\",\n  \"description\": \"DomainName schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-domain-name-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DomainName
---
