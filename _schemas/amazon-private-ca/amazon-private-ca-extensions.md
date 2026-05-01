---
description: Contains X.509 extension information for a certificate.
layout: schema
name: Extensions
properties_list:
- description: ''
  name: CertificatePolicies
  type: object
- description: ''
  name: ExtendedKeyUsage
  type: object
- description: ''
  name: KeyUsage
  type: object
- description: ''
  name: SubjectAlternativeNames
  type: object
- description: ''
  name: CustomExtensions
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-extensions-schema.json
slug: amazon-private-ca-extensions
source_filename: amazon-private-ca-extensions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-extensions-schema.json\",\n  \"title\": \"Extensions\",\n  \"description\": \"Contains X.509 extension information for a certificate.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificatePolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificatePolicyList\"\n        },\n        {\n          \"description\": \"<p>Contains a sequence of one or more policy information terms, each of which consists of an object identifier (OID) and optional qualifiers. For more information, see NIST's definition of <a href=\\\"https://csrc.nist.gov/glossary/term/Object_Identifier\\\">Object Identifier (OID)</a>.</p> <p>In an end-entity certificate, these terms indicate the policy under which the certificate was issued and the purposes for which it\
  \ may be used. In a CA certificate, these terms limit the set of policies for certification paths that include this certificate.</p>\"\n        }\n      ]\n    },\n    \"ExtendedKeyUsage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExtendedKeyUsageList\"\n        },\n        {\n          \"description\": \"Specifies additional purposes for which the certified public key may be used other than basic purposes indicated in the <code>KeyUsage</code> extension.\"\n        }\n      ]\n    },\n    \"KeyUsage\": {\n      \"$ref\": \"#/components/schemas/KeyUsage\"\n    },\n    \"SubjectAlternativeNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneralNameList\"\n        },\n        {\n          \"description\": \"The subject alternative name extension allows identities to be bound to the subject of the certificate. These identities may be included in addition to or in place of the identity in the subject field of the certificate.\"\
  \n        }\n      ]\n    },\n    \"CustomExtensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomExtensionList\"\n        },\n        {\n          \"description\": \"<p/> <p>Contains a sequence of one or more X.509 extensions, each of which consists of an object identifier (OID), a base64-encoded value, and the critical flag. For more information, see the <a href=\\\"https://oidref.com/2.5.29\\\">Global OID reference database.</a> </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-extensions-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: Extensions
---
