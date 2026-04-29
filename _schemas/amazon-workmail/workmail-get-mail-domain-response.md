---
description: GetMailDomainResponse schema from Amazon WorkMail API
layout: schema
name: GetMailDomainResponse
properties_list:
- description: ''
  name: Records
  type: object
- description: ''
  name: IsTestDomain
  type: object
- description: ''
  name: IsDefault
  type: object
- description: ''
  name: OwnershipVerificationStatus
  type: object
- description: ''
  name: DkimVerificationStatus
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-get-mail-domain-response-schema.json
slug: workmail-get-mail-domain-response
source_filename: workmail-get-mail-domain-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Records\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsRecords\"\n        },\n        {\n          \"description\": \"A list of the DNS records that WorkMail recommends adding in your DNS provider for the best user experience. The records configure your domain with DMARC, SPF, DKIM, and direct incoming email traffic to SES. See admin guide for more details.\"\n        }\n      ]\n    },\n    \"IsTestDomain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the domain is a test domain provided by WorkMail, or a custom domain.\"\n        }\n      ]\n    },\n    \"IsDefault\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the domain is the default domain for your organization.\"\
  \n        }\n      ]\n    },\n    \"OwnershipVerificationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsRecordVerificationStatus\"\n        },\n        {\n          \"description\": \" Indicates the status of the domain ownership verification.\"\n        }\n      ]\n    },\n    \"DkimVerificationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsRecordVerificationStatus\"\n        },\n        {\n          \"description\": \"Indicates the status of a DKIM verification.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetMailDomainResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-mail-domain-response-schema.json\",\n  \"description\": \"GetMailDomainResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-mail-domain-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: GetMailDomainResponse
---
