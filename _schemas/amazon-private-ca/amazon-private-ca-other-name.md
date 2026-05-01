---
description: Defines a custom ASN.1 X.400 <code>GeneralName</code> using an object identifier (OID) and value. The OID must satisfy the regular expression shown below. For more information, see NIST's definition of <a href="https://csrc.nist.gov/glossary/term/Object_Identifier">Object Identifier (OID)</a>.
layout: schema
name: OtherName
properties_list:
- description: ''
  name: TypeId
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-other-name-schema.json
slug: amazon-private-ca-other-name
source_filename: amazon-private-ca-other-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-other-name-schema.json\",\n  \"title\": \"OtherName\",\n  \"description\": \"Defines a custom ASN.1 X.400 <code>GeneralName</code> using an object identifier (OID) and value. The OID must satisfy the regular expression shown below. For more information, see NIST's definition of <a href=\\\"https://csrc.nist.gov/glossary/term/Object_Identifier\\\">Object Identifier (OID)</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomObjectIdentifier\"\n        },\n        {\n          \"description\": \"Specifies an OID. \"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String256\"\n        },\n        {\n          \"description\"\
  : \"Specifies an OID value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TypeId\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-other-name-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: OtherName
---
