---
description: Defines a <code>PolicyInformation</code> qualifier. Amazon Web Services Private CA supports the <a href="https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.4">certification practice statement (CPS) qualifier</a> defined in RFC 5280.
layout: schema
name: Qualifier
properties_list:
- description: ''
  name: CpsUri
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-qualifier-schema.json
slug: amazon-private-ca-qualifier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-qualifier-schema.json\",\n  \"title\": \"Qualifier\",\n  \"description\": \"Defines a <code>PolicyInformation</code> qualifier. Amazon Web Services Private CA supports the <a href=\\\"https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.4\\\">certification practice statement (CPS) qualifier</a> defined in RFC 5280. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CpsUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String256\"\n        },\n        {\n          \"description\": \"Contains a pointer to a certification practice statement (CPS) published by the CA.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CpsUri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-qualifier-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: Qualifier
---
