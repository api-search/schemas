---
description: Describes an EWS based availability provider. This is only used as input to the service.
layout: schema
name: EwsAvailabilityProvider
properties_list:
- description: ''
  name: EwsEndpoint
  type: object
- description: ''
  name: EwsUsername
  type: object
- description: ''
  name: EwsPassword
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-ews-availability-provider-schema.json
slug: workmail-ews-availability-provider
source_filename: workmail-ews-availability-provider-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"EwsEndpoint\",\n    \"EwsUsername\",\n    \"EwsPassword\"\n  ],\n  \"properties\": {\n    \"EwsEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The endpoint of the remote EWS server.\"\n        }\n      ]\n    },\n    \"EwsUsername\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalUserName\"\n        },\n        {\n          \"description\": \"The username used to authenticate the remote EWS server.\"\n        }\n      ]\n    },\n    \"EwsPassword\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Password\"\n        },\n        {\n          \"description\": \"The password used to authenticate the remote EWS server.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes an EWS based availability provider. This is only used as input to the service.\"\
  ,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EwsAvailabilityProvider\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-ews-availability-provider-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-ews-availability-provider-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: EwsAvailabilityProvider
---
