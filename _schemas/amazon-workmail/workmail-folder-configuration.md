---
description: The configuration applied to an organization's folders by its retention policy.
layout: schema
name: FolderConfiguration
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Action
  type: object
- description: ''
  name: Period
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-folder-configuration-schema.json
slug: workmail-folder-configuration
source_filename: workmail-folder-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Name\",\n    \"Action\"\n  ],\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FolderName\"\n        },\n        {\n          \"description\": \"The folder name.\"\n        }\n      ]\n    },\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionAction\"\n        },\n        {\n          \"description\": \"The action to take on the folder contents at the end of the folder configuration period.\"\n        }\n      ]\n    },\n    \"Period\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionPeriod\"\n        },\n        {\n          \"description\": \"The number of days for which the folder-configuration action applies.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The configuration applied to an organization's folders by its retention policy.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"FolderConfiguration\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-folder-configuration-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-folder-configuration-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: FolderConfiguration
---
