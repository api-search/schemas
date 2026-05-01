---
description: ListMobileDeviceAccessOverridesRequest schema from Amazon WorkMail API
layout: schema
name: ListMobileDeviceAccessOverridesRequest
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
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-mobile-device-access-overrides-request-schema.json
slug: workmail-list-mobile-device-access-overrides-request
source_filename: workmail-list-mobile-device-access-overrides-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\"\n  ],\n  \"title\": \"ListMobileDeviceAccessOverridesRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization under which to list mobile device access overrides.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityIdentifier\"\n        },\n        {\n          \"description\": \"<p>The WorkMail user under which you list the mobile device access overrides. Accepts the following types of user identities:</p> <ul> <li> <p>User ID: <code>12345678-1234-1234-1234-123456789012</code> or <code>S-1-1-12-1234567890-123456789-123456789-1234</code> </p> </li> <li> <p>Email address: <code>user@domain.tld</code> </p> </li> <li> <p>User name: <code>user</code> </p> </li> </ul>\"\
  \n        }\n      ]\n    },\n    \"DeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceId\"\n        },\n        {\n          \"description\": \"The mobile device to which the access override applies.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. The first call does not require a token.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to return in a single call.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mobile-device-access-overrides-request-schema.json\"\
  ,\n  \"description\": \"ListMobileDeviceAccessOverridesRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mobile-device-access-overrides-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListMobileDeviceAccessOverridesRequest
---
