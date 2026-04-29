---
description: A Learning Manager account
layout: schema
name: Account
properties_list:
- description: Unique account identifier
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-account-schema.json
slug: prime-api-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"A Learning Manager account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique account identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"account\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"dateCreated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Account creation timestamp\"\n        },\n        \"gamificationEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether gamification features are enabled\"\n        },\n        \"locale\": {\n          \"type\": \"string\",\n    \
  \      \"description\": \"Default locale for the account\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Account name\"\n        },\n        \"subdomain\": {\n          \"type\": \"string\",\n          \"description\": \"The Learning Manager subdomain\"\n        },\n        \"timezone\": {\n          \"type\": \"string\",\n          \"description\": \"Default timezone for the account\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-account-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: Account
---
