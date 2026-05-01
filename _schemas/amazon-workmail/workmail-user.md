---
description: The representation of an WorkMail user.
layout: schema
name: User
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
  name: DisplayName
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: UserRole
  type: object
- description: ''
  name: EnabledDate
  type: object
- description: ''
  name: DisabledDate
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-user-schema.json
slug: workmail-user
source_filename: workmail-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the user.\"\n        }\n      ]\n    },\n    \"Email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailAddress\"\n        },\n        {\n          \"description\": \"The email of the user.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"The name of the user.\"\n        }\n      ]\n    },\n    \"DisplayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The display name of the user.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityState\"\
  \n        },\n        {\n          \"description\": \"The state of the user, which can be ENABLED, DISABLED, or DELETED.\"\n        }\n      ]\n    },\n    \"UserRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserRole\"\n        },\n        {\n          \"description\": \"The role of the user.\"\n        }\n      ]\n    },\n    \"EnabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date indicating when the user was enabled for WorkMail use.\"\n        }\n      ]\n    },\n    \"DisabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date indicating when the user was disabled from WorkMail use.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The representation of an WorkMail user.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"User\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-user-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-user-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: User
---
