---
description: Defines the X.500 relative distinguished name (RDN).
layout: schema
name: CustomAttribute
properties_list:
- description: ''
  name: ObjectIdentifier
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-custom-attribute-schema.json
slug: amazon-private-ca-custom-attribute
source_filename: amazon-private-ca-custom-attribute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-custom-attribute-schema.json\",\n  \"title\": \"CustomAttribute\",\n  \"description\": \"Defines the X.500 relative distinguished name (RDN).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObjectIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomObjectIdentifier\"\n        },\n        {\n          \"description\": \"Specifies the object identifier (OID) of the attribute type of the relative distinguished name (RDN).\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String1To256\"\n        },\n        {\n          \"description\": \"<p/> <p>Specifies the attribute value of relative distinguished name (RDN).</p>\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"ObjectIdentifier\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-custom-attribute-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: CustomAttribute
---
