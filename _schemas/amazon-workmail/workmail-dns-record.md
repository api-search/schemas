---
description: A DNS record uploaded to your DNS provider.
layout: schema
name: DnsRecord
properties_list:
- description: ''
  name: Type
  type: object
- description: ''
  name: Hostname
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-dns-record-schema.json
slug: workmail-dns-record
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The RFC 1035 record type. Possible values: <code>CNAME</code>, <code>A</code>, <code>MX</code>.\"\n        }\n      ]\n    },\n    \"Hostname\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The DNS hostname.- For example, <code>domain.example.com</code>.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The value returned by the DNS for a query to that hostname and record type.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A DNS record uploaded to your DNS provider.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"\
  title\": \"DnsRecord\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-dns-record-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-dns-record-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DnsRecord
---
