---
description: ListMobileDeviceAccessRulesRequest schema from Amazon WorkMail API
layout: schema
name: ListMobileDeviceAccessRulesRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-mobile-device-access-rules-request-schema.json
slug: workmail-list-mobile-device-access-rules-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\"\n  ],\n  \"title\": \"ListMobileDeviceAccessRulesRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization for which to list the rules.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mobile-device-access-rules-request-schema.json\",\n  \"description\": \"ListMobileDeviceAccessRulesRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mobile-device-access-rules-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListMobileDeviceAccessRulesRequest
---
