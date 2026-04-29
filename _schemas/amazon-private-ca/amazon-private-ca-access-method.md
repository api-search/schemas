---
description: Describes the type and format of extension access. Only one of <code>CustomObjectIdentifier</code> or <code>AccessMethodType</code> may be provided. Providing both results in <code>InvalidArgsException</code>.
layout: schema
name: AccessMethod
properties_list:
- description: ''
  name: CustomObjectIdentifier
  type: object
- description: ''
  name: AccessMethodType
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-access-method-schema.json
slug: amazon-private-ca-access-method
source_filename: amazon-private-ca-access-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-access-method-schema.json\",\n  \"title\": \"AccessMethod\",\n  \"description\": \"Describes the type and format of extension access. Only one of <code>CustomObjectIdentifier</code> or <code>AccessMethodType</code> may be provided. Providing both results in <code>InvalidArgsException</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomObjectIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomObjectIdentifier\"\n        },\n        {\n          \"description\": \"An object identifier (OID) specifying the <code>AccessMethod</code>. The OID must satisfy the regular expression shown below. For more information, see NIST's definition of <a href=\\\"https://csrc.nist.gov/glossary/term/Object_Identifier\\\">Object Identifier (OID)</a>.\"\
  \n        }\n      ]\n    },\n    \"AccessMethodType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessMethodType\"\n        },\n        {\n          \"description\": \"Specifies the <code>AccessMethod</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-access-method-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: AccessMethod
---
