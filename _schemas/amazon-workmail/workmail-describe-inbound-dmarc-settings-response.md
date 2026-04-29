---
description: DescribeInboundDmarcSettingsResponse schema from Amazon WorkMail API
layout: schema
name: DescribeInboundDmarcSettingsResponse
properties_list:
- description: ''
  name: Enforced
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-describe-inbound-dmarc-settings-response-schema.json
slug: workmail-describe-inbound-dmarc-settings-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enforced\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Lists the enforcement setting of the applied policy.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeInboundDmarcSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-inbound-dmarc-settings-response-schema.json\",\n  \"description\": \"DescribeInboundDmarcSettingsResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-inbound-dmarc-settings-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeInboundDmarcSettingsResponse
---
