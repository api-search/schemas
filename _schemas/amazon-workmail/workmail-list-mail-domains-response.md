---
description: ListMailDomainsResponse schema from Amazon WorkMail API
layout: schema
name: ListMailDomainsResponse
properties_list:
- description: ''
  name: MailDomains
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-mail-domains-response-schema.json
slug: workmail-list-mail-domains-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MailDomains\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailDomains\"\n        },\n        {\n          \"description\": \"The list of mail domain summaries, specifying domains that exist in the specified WorkMail organization, along with the information about whether the domain is or isn't the default.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. The value becomes <code>null</code> when there are no more results to return.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListMailDomainsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mail-domains-response-schema.json\"\
  ,\n  \"description\": \"ListMailDomainsResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mail-domains-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListMailDomainsResponse
---
