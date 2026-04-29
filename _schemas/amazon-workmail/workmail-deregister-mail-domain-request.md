---
description: DeregisterMailDomainRequest schema from Amazon WorkMail API
layout: schema
name: DeregisterMailDomainRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: DomainName
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-deregister-mail-domain-request-schema.json
slug: workmail-deregister-mail-domain-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"DomainName\"\n  ],\n  \"title\": \"DeregisterMailDomainRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization for which the domain will be deregistered.\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailDomainName\"\n        },\n        {\n          \"description\": \"The domain to deregister in WorkMail and SES.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-deregister-mail-domain-request-schema.json\",\n  \"description\": \"DeregisterMailDomainRequest schema from Amazon WorkMail\
  \ API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-deregister-mail-domain-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeregisterMailDomainRequest
---
