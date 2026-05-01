---
description: AssociateMemberToGroupRequest schema from Amazon WorkMail API
layout: schema
name: AssociateMemberToGroupRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: GroupId
  type: object
- description: ''
  name: MemberId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-associate-member-to-group-request-schema.json
slug: workmail-associate-member-to-group-request
source_filename: workmail-associate-member-to-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"GroupId\",\n    \"MemberId\"\n  ],\n  \"title\": \"AssociateMemberToGroupRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The organization under which the group exists.\"\n        }\n      ]\n    },\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The group to which the member (user or group) is associated.\"\n        }\n      ]\n    },\n    \"MemberId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The member (user or group) to associate to the group.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-associate-member-to-group-request-schema.json\",\n  \"description\": \"AssociateMemberToGroupRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-associate-member-to-group-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: AssociateMemberToGroupRequest
---
