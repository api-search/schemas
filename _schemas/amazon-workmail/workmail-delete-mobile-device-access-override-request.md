---
description: DeleteMobileDeviceAccessOverrideRequest schema from Amazon WorkMail API
layout: schema
name: DeleteMobileDeviceAccessOverrideRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: UserId
  type: object
- description: ''
  name: DeviceId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delete-mobile-device-access-override-request-schema.json
slug: workmail-delete-mobile-device-access-override-request
source_filename: workmail-delete-mobile-device-access-override-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"UserId\",\n    \"DeviceId\"\n  ],\n  \"title\": \"DeleteMobileDeviceAccessOverrideRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization for which the access override will be deleted.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityIdentifier\"\n        },\n        {\n          \"description\": \"<p>The WorkMail user for which you want to delete the override. Accepts the following types of user identities:</p> <ul> <li> <p>User ID: <code>12345678-1234-1234-1234-123456789012</code> or <code>S-1-1-12-1234567890-123456789-123456789-1234</code> </p> </li> <li> <p>Email address: <code>user@domain.tld</code> </p> </li> <li> <p>User name: <code>user</code>\
  \ </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"DeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceId\"\n        },\n        {\n          \"description\": \"The mobile device for which you delete the override. <code>DeviceId</code> is case insensitive.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-mobile-device-access-override-request-schema.json\",\n  \"description\": \"DeleteMobileDeviceAccessOverrideRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-mobile-device-access-override-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeleteMobileDeviceAccessOverrideRequest
---
