---
description: Provides access information used by the <code>authorityInfoAccess</code> and <code>subjectInfoAccess</code> extensions described in <a href="https://datatracker.ietf.org/doc/html/rfc5280">RFC 5280</a>.
layout: schema
name: AccessDescription
properties_list:
- description: ''
  name: AccessMethod
  type: object
- description: ''
  name: AccessLocation
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-access-description-schema.json
slug: amazon-private-ca-access-description
source_filename: amazon-private-ca-access-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-access-description-schema.json\",\n  \"title\": \"AccessDescription\",\n  \"description\": \"Provides access information used by the <code>authorityInfoAccess</code> and <code>subjectInfoAccess</code> extensions described in <a href=\\\"https://datatracker.ietf.org/doc/html/rfc5280\\\">RFC 5280</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessMethod\"\n        },\n        {\n          \"description\": \"The type and format of <code>AccessDescription</code> information.\"\n        }\n      ]\n    },\n    \"AccessLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneralName\"\n        },\n        {\n          \"description\": \"The location\
  \ of <code>AccessDescription</code> information.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessMethod\",\n    \"AccessLocation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-access-description-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: AccessDescription
---
