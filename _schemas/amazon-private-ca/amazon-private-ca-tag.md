---
description: Tags are labels that you can use to identify and organize your private CAs. Each tag consists of a key and an optional value. You can associate up to 50 tags with a private CA. To add one or more tags to a private CA, call the <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_TagCertificateAuthority.html">TagCertificateAuthority</a> action. To remove a tag, call the <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_UntagCertificateAuthority.html">UntagCertificateAuthority</a> action.
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-tag-schema.json
slug: amazon-private-ca-tag
source_filename: amazon-private-ca-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Tags are labels that you can use to identify and organize your private CAs. Each tag consists of a key and an optional value. You can associate up to 50 tags with a private CA. To add one or more tags to a private CA, call the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_TagCertificateAuthority.html\\\">TagCertificateAuthority</a> action. To remove a tag, call the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_UntagCertificateAuthority.html\\\">UntagCertificateAuthority</a> action. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"\
  description\": \"Key (name) of the tag.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \"Value of the tag.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-tag-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: Tag
---
