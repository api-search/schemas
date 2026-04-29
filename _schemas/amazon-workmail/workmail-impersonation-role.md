---
description: An impersonation role for the given WorkMail organization.
layout: schema
name: ImpersonationRole
properties_list:
- description: ''
  name: ImpersonationRoleId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: DateCreated
  type: object
- description: ''
  name: DateModified
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-impersonation-role-schema.json
slug: workmail-impersonation-role
source_filename: workmail-impersonation-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImpersonationRoleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleId\"\n        },\n        {\n          \"description\": \"The identifier of the impersonation role.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleName\"\n        },\n        {\n          \"description\": \"The impersonation role name.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleType\"\n        },\n        {\n          \"description\": \"The impersonation role type.\"\n        }\n      ]\n    },\n    \"DateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date when the impersonation role was created.\"\n        }\n \
  \     ]\n    },\n    \"DateModified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date when the impersonation role was last modified.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An impersonation role for the given WorkMail organization.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImpersonationRole\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-impersonation-role-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-impersonation-role-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ImpersonationRole
---
