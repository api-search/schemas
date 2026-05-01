---
description: The name of the attribute, which is one of the values defined in the UserAttribute enumeration.
layout: schema
name: Delegate
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delegate-schema.json
slug: workmail-delegate
source_filename: workmail-delegate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Id\",\n    \"Type\"\n  ],\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier for the user or group associated as the resource's delegate.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberType\"\n        },\n        {\n          \"description\": \"The type of the delegate: user or group.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The name of the attribute, which is one of the values defined in the UserAttribute enumeration.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Delegate\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delegate-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delegate-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: Delegate
---
