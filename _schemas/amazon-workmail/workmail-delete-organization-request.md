---
description: DeleteOrganizationRequest schema from Amazon WorkMail API
layout: schema
name: DeleteOrganizationRequest
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: DeleteDirectory
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delete-organization-request-schema.json
slug: workmail-delete-organization-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"DeleteDirectory\"\n  ],\n  \"title\": \"DeleteOrganizationRequest\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token associated with the request.\"\n        }\n      ]\n    },\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The organization ID.\"\n        }\n      ]\n    },\n    \"DeleteDirectory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"If true, deletes the AWS Directory Service directory associated with the organization.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-organization-request-schema.json\",\n  \"description\": \"DeleteOrganizationRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-organization-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeleteOrganizationRequest
---
