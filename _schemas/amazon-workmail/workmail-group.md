---
description: The representation of an WorkMail group.
layout: schema
name: Group
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Email
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: EnabledDate
  type: object
- description: ''
  name: DisabledDate
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-group-schema.json
slug: workmail-group
source_filename: workmail-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the group.\"\n        }\n      ]\n    },\n    \"Email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailAddress\"\n        },\n        {\n          \"description\": \"The email of the group.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupName\"\n        },\n        {\n          \"description\": \"The name of the group.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityState\"\n        },\n        {\n          \"description\": \"The state of the group, which can be ENABLED, DISABLED, or DELETED.\"\n        }\n      ]\n    },\n    \"EnabledDate\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date indicating when the group was enabled for WorkMail use.\"\n        }\n      ]\n    },\n    \"DisabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date indicating when the group was disabled from WorkMail use.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The representation of an WorkMail group.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-group-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-group-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: Group
---
