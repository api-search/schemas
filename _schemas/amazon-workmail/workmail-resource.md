---
description: The representation of a resource.
layout: schema
name: Resource
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
  name: Type
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
schema_file: json-schema/workmail-resource-schema.json
slug: workmail-resource
source_filename: workmail-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the resource.\"\n        }\n      ]\n    },\n    \"Email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailAddress\"\n        },\n        {\n          \"description\": \"The email of the resource.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the resource.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The type of the resource: equipment or room.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/EntityState\"\n        },\n        {\n          \"description\": \"The state of the resource, which can be ENABLED, DISABLED, or DELETED.\"\n        }\n      ]\n    },\n    \"EnabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date indicating when the resource was enabled for WorkMail use.\"\n        }\n      ]\n    },\n    \"DisabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date indicating when the resource was disabled from WorkMail use.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The representation of a resource.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Resource\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-resource-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-resource-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: Resource
---
