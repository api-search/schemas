---
description: Describes an Electronic Data Interchange (EDI) entity as described in as defined in <a href="https://datatracker.ietf.org/doc/html/rfc5280">Subject Alternative Name</a> in RFC 5280.
layout: schema
name: EdiPartyName
properties_list:
- description: ''
  name: PartyName
  type: object
- description: ''
  name: NameAssigner
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-edi-party-name-schema.json
slug: amazon-private-ca-edi-party-name
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-edi-party-name-schema.json\",\n  \"title\": \"EdiPartyName\",\n  \"description\": \"Describes an Electronic Data Interchange (EDI) entity as described in as defined in <a href=\\\"https://datatracker.ietf.org/doc/html/rfc5280\\\">Subject Alternative Name</a> in RFC 5280.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PartyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String256\"\n        },\n        {\n          \"description\": \"Specifies the party name.\"\n        }\n      ]\n    },\n    \"NameAssigner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String256\"\n        },\n        {\n          \"description\": \"Specifies the name assigner.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  PartyName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-edi-party-name-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: EdiPartyName
---
