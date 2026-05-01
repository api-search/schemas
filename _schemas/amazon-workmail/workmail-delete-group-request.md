---
description: DeleteGroupRequest schema from Amazon WorkMail API
layout: schema
name: DeleteGroupRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: GroupId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delete-group-request-schema.json
slug: workmail-delete-group-request
source_filename: workmail-delete-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"GroupId\"\n  ],\n  \"title\": \"DeleteGroupRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The organization that contains the group.\"\n        }\n      ]\n    },\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the group to be deleted.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-group-request-schema.json\",\n  \"description\": \"DeleteGroupRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-group-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeleteGroupRequest
---
