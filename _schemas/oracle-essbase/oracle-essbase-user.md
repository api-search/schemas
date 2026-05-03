---
description: An Oracle Essbase user account with role-based access control. Users are assigned service roles (User, Power User, or Service Administrator) and can belong to groups for simplified permission management.
layout: schema
name: Oracle Essbase User
properties_list:
- description: Unique user identifier used for login and API references.
  name: id
  type: string
- description: 'User display name. Maximum 256 characters. Special characters not permitted: ; , = + * ? [ ] | < > \ " '' / space tab.'
  name: name
  type: string
- description: User email address for notifications and account recovery.
  name: email
  type: string
- description: User password. Write-only; not returned in API responses.
  name: password
  type: string
- description: Service-level role determining the user's base permissions. User has read access. Power User can create and manage applications. Service Administrator has full administrative control.
  name: role
  type: string
- description: Authentication token for the user session.
  name: token
  type: string
- description: List of group names the user belongs to.
  name: groups
  type: array
- description: HATEOAS navigation links.
  name: links
  type: array
provider_name: Oracle Essbase
provider_slug: oracle-essbase
schema_file: json-schema/oracle-essbase-user-schema.json
slug: oracle-essbase-user
source_filename: oracle-essbase-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"oracle-essbase-user-schema.json\",\n  \"title\": \"Oracle Essbase User\",\n  \"description\": \"An Oracle Essbase user account with role-based access control. Users are assigned service roles (User, Power User, or Service Administrator) and can belong to groups for simplified permission management.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique user identifier used for login and API references.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User display name. Maximum 256 characters. Special characters not permitted: ; , = + * ? [ ] | < > \\\\ \\\" ' / space tab.\",\n      \"maxLength\": 256\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email address for notifications and account recovery.\"\n    },\n    \"password\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"User password. Write-only; not returned in API responses.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Service-level role determining the user's base permissions. User has read access. Power User can create and manage applications. Service Administrator has full administrative control.\",\n      \"enum\": [\"User\", \"Power User\", \"Service Administrator\"]\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication token for the user session.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"List of group names the user belongs to.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"HATEOAS navigation links.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Link\"\n      }\n    }\n  },\n  \"required\": [\"id\"],\n  \"$defs\": {\n \
  \   \"Link\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS navigation link.\",\n      \"properties\": {\n        \"rel\": {\n          \"type\": \"string\",\n          \"description\": \"Link relation type.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Link URL.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method for this link.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Media type of the linked resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/json-schema/oracle-essbase-user-schema.json
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
title: Oracle Essbase User
---
