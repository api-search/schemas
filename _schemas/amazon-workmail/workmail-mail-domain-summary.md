---
description: The data for a given domain.
layout: schema
name: MailDomainSummary
properties_list:
- description: ''
  name: DomainName
  type: object
- description: ''
  name: DefaultDomain
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-mail-domain-summary-schema.json
slug: workmail-mail-domain-summary
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The domain name.\"\n        }\n      ]\n    },\n    \"DefaultDomain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the domain is default or not.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The data for a given domain.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MailDomainSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-mail-domain-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-mail-domain-summary-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: MailDomainSummary
---
