---
description: Describes an ASN.1 X.400 <code>GeneralName</code> as defined in <a href="https://datatracker.ietf.org/doc/html/rfc5280">RFC 5280</a>. Only one of the following naming options should be provided. Providing more than one option results in an <code>InvalidArgsException</code> error.
layout: schema
name: GeneralName
properties_list:
- description: ''
  name: OtherName
  type: object
- description: ''
  name: Rfc822Name
  type: object
- description: ''
  name: DnsName
  type: object
- description: ''
  name: DirectoryName
  type: object
- description: ''
  name: EdiPartyName
  type: object
- description: ''
  name: UniformResourceIdentifier
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: RegisteredId
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-general-name-schema.json
slug: amazon-private-ca-general-name
source_filename: amazon-private-ca-general-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-general-name-schema.json\",\n  \"title\": \"GeneralName\",\n  \"description\": \"Describes an ASN.1 X.400 <code>GeneralName</code> as defined in <a href=\\\"https://datatracker.ietf.org/doc/html/rfc5280\\\">RFC 5280</a>. Only one of the following naming options should be provided. Providing more than one option results in an <code>InvalidArgsException</code> error.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OtherName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OtherName\"\n        },\n        {\n          \"description\": \"Represents <code>GeneralName</code> using an <code>OtherName</code> object.\"\n        }\n      ]\n    },\n    \"Rfc822Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String256\"\
  \n        },\n        {\n          \"description\": \"Represents <code>GeneralName</code> as an <a href=\\\"https://datatracker.ietf.org/doc/html/rfc822\\\">RFC 822</a> email address.\"\n        }\n      ]\n    },\n    \"DnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String253\"\n        },\n        {\n          \"description\": \"Represents <code>GeneralName</code> as a DNS name.\"\n        }\n      ]\n    },\n    \"DirectoryName\": {\n      \"$ref\": \"#/components/schemas/ASN1Subject\"\n    },\n    \"EdiPartyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EdiPartyName\"\n        },\n        {\n          \"description\": \"Represents <code>GeneralName</code> as an <code>EdiPartyName</code> object.\"\n        }\n      ]\n    },\n    \"UniformResourceIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String253\"\n        },\n        {\n          \"description\": \"Represents\
  \ <code>GeneralName</code> as a URI.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String39\"\n        },\n        {\n          \"description\": \"Represents <code>GeneralName</code> as an IPv4 or IPv6 address.\"\n        }\n      ]\n    },\n    \"RegisteredId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomObjectIdentifier\"\n        },\n        {\n          \"description\": \" Represents <code>GeneralName</code> as an object identifier (OID).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-general-name-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: GeneralName
---
