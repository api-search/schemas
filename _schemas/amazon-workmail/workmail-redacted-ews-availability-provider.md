---
description: Describes an EWS based availability provider when returned from the service. It does not contain the password of the endpoint.
layout: schema
name: RedactedEwsAvailabilityProvider
properties_list:
- description: ''
  name: EwsEndpoint
  type: object
- description: ''
  name: EwsUsername
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-redacted-ews-availability-provider-schema.json
slug: workmail-redacted-ews-availability-provider
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"EwsEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The endpoint of the remote EWS server.\"\n        }\n      ]\n    },\n    \"EwsUsername\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalUserName\"\n        },\n        {\n          \"description\": \"The username used to authenticate the remote EWS server.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes an EWS based availability provider when returned from the service. It does not contain the password of the endpoint.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RedactedEwsAvailabilityProvider\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-redacted-ews-availability-provider-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-redacted-ews-availability-provider-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: RedactedEwsAvailabilityProvider
---
