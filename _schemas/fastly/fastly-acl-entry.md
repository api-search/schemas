---
description: An individual entry within a Fastly Access Control List (ACL), representing an IP address or CIDR range used for edge access control. ACL entries are versionless and take effect immediately without requiring a new service version.
layout: schema
name: Fastly ACL Entry
properties_list:
- description: The alphanumeric string identifying the ACL entry.
  name: id
  type: string
- description: The alphanumeric string identifying the parent ACL.
  name: acl_id
  type: string
- description: An IP address or the first address of a CIDR range.
  name: ip
  type: string
- description: The CIDR subnet mask for IP ranges. A value of 32 indicates a single IP address.
  name: subnet
  type: integer
- description: Whether the entry is negated (0 = match, 1 = do not match).
  name: negated
  type: integer
- description: A freeform descriptive note about the ACL entry.
  name: comment
  type: string
- description: The date and time the entry was created.
  name: created_at
  type: string
- description: The date and time the entry was last updated.
  name: updated_at
  type: string
- description: The date and time the entry was deleted.
  name: deleted_at
  type:
  - string
  - 'null'
provider_name: fastly
provider_slug: fastly
schema_file: json-schema/fastly-acl-entry-schema.json
slug: fastly-acl-entry
source_filename: fastly-acl-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/fastly/acl-entry.json\",\n  \"title\": \"Fastly ACL Entry\",\n  \"description\": \"An individual entry within a Fastly Access Control List (ACL), representing an IP address or CIDR range used for edge access control. ACL entries are versionless and take effect immediately without requiring a new service version.\",\n  \"type\": \"object\",\n  \"required\": [\"ip\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The alphanumeric string identifying the ACL entry.\"\n    },\n    \"acl_id\": {\n      \"type\": \"string\",\n      \"description\": \"The alphanumeric string identifying the parent ACL.\"\n    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"description\": \"An IP address or the first address of a CIDR range.\",\n      \"format\": \"ipv4\"\n    },\n    \"subnet\": {\n      \"type\": \"integer\",\n  \
  \    \"description\": \"The CIDR subnet mask for IP ranges. A value of 32 indicates a single IP address.\",\n      \"minimum\": 0,\n      \"maximum\": 128\n    },\n    \"negated\": {\n      \"type\": \"integer\",\n      \"description\": \"Whether the entry is negated (0 = match, 1 = do not match).\",\n      \"enum\": [0, 1]\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"A freeform descriptive note about the ACL entry.\",\n      \"maxLength\": 1024\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the entry was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the entry was last updated.\"\n    },\n    \"deleted_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the entry was deleted.\"\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fastly/refs/heads/main/json-schema/fastly-acl-entry-schema.json
tags: []
title: Fastly ACL Entry
---
