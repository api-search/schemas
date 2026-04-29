---
description: TagKeyList schema
layout: schema
name: TagKeyList
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-tag-key-list-schema.json
slug: incident-manager-tag-key-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-tag-key-list-schema.json\",\n  \"title\": \"TagKeyList\",\n  \"description\": \"TagKeyList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^(?!aws:)[A-Za-z0-9 _=@:.+-/]+$\",\n    \"minLength\": 1,\n    \"maxLength\": 128\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-tag-key-list-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: TagKeyList
---
