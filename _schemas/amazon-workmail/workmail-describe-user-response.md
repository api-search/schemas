---
description: DescribeUserResponse schema from Amazon WorkMail API
layout: schema
name: DescribeUserResponse
properties_list:
- description: ''
  name: UserId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Email
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
schema_file: json-schema/workmail-describe-user-response-schema.json
slug: workmail-describe-user-response
source_filename: workmail-describe-user-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier for the described user.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"The name for the user.\"\n        }\n      ]\n    },\n    \"Email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailAddress\"\n        },\n        {\n          \"description\": \"The email of the user.\"\n        }\n      ]\n    },\n    \"DisplayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The display name of the user.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/EntityState\"\n        },\n        {\n          \"description\": \"The state of a user: enabled (registered to WorkMail) or disabled (deregistered or never registered to WorkMail).\"\n        }\n      ]\n    },\n    \"UserRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserRole\"\n        },\n        {\n          \"description\": \"In certain cases, other entities are modeled as users. If interoperability is enabled, resources are imported into WorkMail as users. Because different WorkMail organizations rely on different directory types, administrators can distinguish between an unregistered user (account is disabled and has a user role) and the directory administrators. The values are USER, RESOURCE, and SYSTEM_USER.\"\n        }\n      ]\n    },\n    \"EnabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date\
  \ and time at which the user was enabled for WorkMailusage, in UNIX epoch time format.\"\n        }\n      ]\n    },\n    \"DisabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time at which the user was disabled for WorkMail usage, in UNIX epoch time format.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeUserResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-user-response-schema.json\",\n  \"description\": \"DescribeUserResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-user-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeUserResponse
---
