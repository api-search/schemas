---
description: PutInboundDmarcSettingsRequest schema from Amazon WorkMail API
layout: schema
name: PutInboundDmarcSettingsRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: Enforced
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-put-inbound-dmarc-settings-request-schema.json
slug: workmail-put-inbound-dmarc-settings-request
source_filename: workmail-put-inbound-dmarc-settings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"Enforced\"\n  ],\n  \"title\": \"PutInboundDmarcSettingsRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The ID of the organization that you are applying the DMARC policy to.\"\n        }\n      ]\n    },\n    \"Enforced\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Enforces or suspends a policy after it's applied.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-put-inbound-dmarc-settings-request-schema.json\",\n  \"description\": \"PutInboundDmarcSettingsRequest schema from Amazon\
  \ WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-put-inbound-dmarc-settings-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: PutInboundDmarcSettingsRequest
---
