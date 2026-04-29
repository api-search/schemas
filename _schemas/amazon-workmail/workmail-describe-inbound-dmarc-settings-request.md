---
description: DescribeInboundDmarcSettingsRequest schema from Amazon WorkMail API
layout: schema
name: DescribeInboundDmarcSettingsRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-describe-inbound-dmarc-settings-request-schema.json
slug: workmail-describe-inbound-dmarc-settings-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\"\n  ],\n  \"title\": \"DescribeInboundDmarcSettingsRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"Lists the ID of the given organization.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-inbound-dmarc-settings-request-schema.json\",\n  \"description\": \"DescribeInboundDmarcSettingsRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-inbound-dmarc-settings-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeInboundDmarcSettingsRequest
---
