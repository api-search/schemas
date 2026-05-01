---
description: <p/> <p>Specifies the X.509 extension information for a certificate.</p> <p>Extensions present in <code>CustomExtensions</code> follow the <code>ApiPassthrough</code> <a href="https://docs.aws.amazon.com/privateca/latest/userguide/UsingTemplates.html#template-order-of-operations">template rules</a>. </p>
layout: schema
name: CustomExtension
properties_list:
- description: ''
  name: ObjectIdentifier
  type: object
- description: ''
  name: Value
  type: object
- description: ''
  name: Critical
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-custom-extension-schema.json
slug: amazon-private-ca-custom-extension
source_filename: amazon-private-ca-custom-extension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-custom-extension-schema.json\",\n  \"title\": \"CustomExtension\",\n  \"description\": \"<p/> <p>Specifies the X.509 extension information for a certificate.</p> <p>Extensions present in <code>CustomExtensions</code> follow the <code>ApiPassthrough</code> <a href=\\\"https://docs.aws.amazon.com/privateca/latest/userguide/UsingTemplates.html#template-order-of-operations\\\">template rules</a>. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObjectIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomObjectIdentifier\"\n        },\n        {\n          \"description\": \"<p/> <p>Specifies the object identifier (OID) of the X.509 extension. For more information, see the <a href=\\\"https://oidref.com/2.5.29\\\">Global OID reference\
  \ database.</a> </p>\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Base64String1To4096\"\n        },\n        {\n          \"description\": \"<p/> <p>Specifies the base64-encoded value of the X.509 extension.</p>\"\n        }\n      ]\n    },\n    \"Critical\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p/> <p>Specifies the critical flag of the X.509 extension.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ObjectIdentifier\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-custom-extension-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: CustomExtension
---
