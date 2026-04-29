---
description: RegisterMailDomainRequest schema from Amazon WorkMail API
layout: schema
name: RegisterMailDomainRequest
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: DomainName
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-register-mail-domain-request-schema.json
slug: workmail-register-mail-domain-request
source_filename: workmail-register-mail-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"DomainName\"\n  ],\n  \"title\": \"RegisterMailDomainRequest\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyClientToken\"\n        },\n        {\n          \"description\": \"Idempotency token used when retrying requests.\"\n        }\n      ]\n    },\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization under which you're creating the domain.\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailDomainName\"\n        },\n        {\n          \"description\": \"The name of the mail domain to create in WorkMail and SES.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-register-mail-domain-request-schema.json\",\n  \"description\": \"RegisterMailDomainRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-register-mail-domain-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: RegisterMailDomainRequest
---
