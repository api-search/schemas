---
description: ListMobileDeviceAccessOverridesResponse schema from Amazon WorkMail API
layout: schema
name: ListMobileDeviceAccessOverridesResponse
properties_list:
- description: ''
  name: Overrides
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-mobile-device-access-overrides-response-schema.json
slug: workmail-list-mobile-device-access-overrides-response
source_filename: workmail-list-mobile-device-access-overrides-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Overrides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessOverridesList\"\n        },\n        {\n          \"description\": \"The list of mobile device access overrides that exist for the specified WorkMail organization and user.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. The value is \\u201cnull\\u201d when there are no more results to return.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListMobileDeviceAccessOverridesResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mobile-device-access-overrides-response-schema.json\"\
  ,\n  \"description\": \"ListMobileDeviceAccessOverridesResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mobile-device-access-overrides-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListMobileDeviceAccessOverridesResponse
---
