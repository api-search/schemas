---
description: A role in a DreamFactory instance that defines service access permissions and can be assigned to users and applications for role-based access control.
layout: schema
name: DreamFactory Role
properties_list:
- description: Unique identifier for the role.
  name: id
  type: integer
- description: Name of the role.
  name: name
  type: string
- description: Description of the role.
  name: description
  type: string
- description: Whether the role is active.
  name: is_active
  type: boolean
- description: Service access permissions assigned to the role.
  name: role_service_access_by_role_id
  type: array
- description: Timestamp when the role was created.
  name: created_date
  type: string
- description: Timestamp when the role was last modified.
  name: last_modified_date
  type: string
provider_name: DreamFactory
provider_slug: dreamfactory
schema_file: json-schema/dreamfactory-role.json
slug: dreamfactory-role
source_filename: dreamfactory-role.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/json-schema/dreamfactory-role.json\",\n  \"title\": \"DreamFactory Role\",\n  \"description\": \"A role in a DreamFactory instance that defines service access permissions and can be assigned to users and applications for role-based access control.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the role.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the role.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the role.\"\n    },\n    \"is_active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the role is active.\"\n    },\n    \"role_service_access_by_role_id\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Service access permissions assigned to the role.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"service_id\": {\n            \"type\": \"integer\",\n            \"description\": \"ID of the service this access rule applies to.\"\n          },\n          \"component\": {\n            \"type\": \"string\",\n            \"description\": \"Service component path the rule applies to.\"\n          },\n          \"verb_mask\": {\n            \"type\": \"integer\",\n            \"description\": \"Bitmask of allowed HTTP verbs.\"\n          },\n          \"requestor_mask\": {\n            \"type\": \"integer\",\n            \"description\": \"Bitmask of allowed requestor types.\"\n          },\n          \"filters\": {\n            \"type\": \"array\",\n            \"description\": \"Filters applied to the access rule.\",\n            \"items\": {\n              \"type\": \"object\"\n            }\n          },\n          \"filter_op\": {\n   \
  \         \"type\": \"string\",\n            \"description\": \"Logical operator for combining filters.\"\n          }\n        }\n      }\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the role was created.\"\n    },\n    \"last_modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the role was last modified.\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/json-schema/dreamfactory-role.json
tags:
- Automation
- Deployment
- Documentation
- Generation
- Security
title: DreamFactory Role
---
