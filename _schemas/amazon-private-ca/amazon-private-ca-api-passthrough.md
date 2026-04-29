---
description: <p>Contains X.509 certificate information to be placed in an issued certificate. An <code>APIPassthrough</code> or <code>APICSRPassthrough</code> template variant must be selected, or else this parameter is ignored. </p> <p>If conflicting or duplicate certificate information is supplied from other sources, Amazon Web Services Private CA applies <a href="https://docs.aws.amazon.com/privateca/latest/userguide/UsingTemplates.html#template-order-of-operations">order of operation rules</a> to determine what information is used.</p>
layout: schema
name: ApiPassthrough
properties_list:
- description: ''
  name: Extensions
  type: object
- description: ''
  name: Subject
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-api-passthrough-schema.json
slug: amazon-private-ca-api-passthrough
source_filename: amazon-private-ca-api-passthrough-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-api-passthrough-schema.json\",\n  \"title\": \"ApiPassthrough\",\n  \"description\": \"<p>Contains X.509 certificate information to be placed in an issued certificate. An <code>APIPassthrough</code> or <code>APICSRPassthrough</code> template variant must be selected, or else this parameter is ignored. </p> <p>If conflicting or duplicate certificate information is supplied from other sources, Amazon Web Services Private CA applies <a href=\\\"https://docs.aws.amazon.com/privateca/latest/userguide/UsingTemplates.html#template-order-of-operations\\\">order of operation rules</a> to determine what information is used.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Extensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Extensions\"\n     \
  \   },\n        {\n          \"description\": \"Specifies X.509 extension information for a certificate.\"\n        }\n      ]\n    },\n    \"Subject\": {\n      \"$ref\": \"#/components/schemas/ASN1Subject\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-api-passthrough-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: ApiPassthrough
---
