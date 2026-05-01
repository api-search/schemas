---
description: DeregisterFromWorkMailRequest schema from Amazon WorkMail API
layout: schema
name: DeregisterFromWorkMailRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: EntityId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-deregister-from-work-mail-request-schema.json
slug: workmail-deregister-from-work-mail-request
source_filename: workmail-deregister-from-work-mail-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"EntityId\"\n  ],\n  \"title\": \"DeregisterFromWorkMailRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier for the organization under which the WorkMail entity exists.\"\n        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier for the member (user or group) to be updated.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-deregister-from-work-mail-request-schema.json\",\n  \"description\": \"DeregisterFromWorkMailRequest\
  \ schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-deregister-from-work-mail-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeregisterFromWorkMailRequest
---
