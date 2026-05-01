---
description: CreateGroupRequest schema from Amazon WorkMail API
layout: schema
name: CreateGroupRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-create-group-request-schema.json
slug: workmail-create-group-request
source_filename: workmail-create-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"Name\"\n  ],\n  \"title\": \"CreateGroupRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The organization under which the group is to be created.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupName\"\n        },\n        {\n          \"description\": \"The name of the group.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-group-request-schema.json\",\n  \"description\": \"CreateGroupRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-group-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: CreateGroupRequest
---
