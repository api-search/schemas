---
description: Defines the X.509 <code>CertificatePolicies</code> extension.
layout: schema
name: PolicyInformation
properties_list:
- description: ''
  name: CertPolicyId
  type: object
- description: ''
  name: PolicyQualifiers
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-policy-information-schema.json
slug: amazon-private-ca-policy-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-policy-information-schema.json\",\n  \"title\": \"PolicyInformation\",\n  \"description\": \"Defines the X.509 <code>CertificatePolicies</code> extension.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertPolicyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomObjectIdentifier\"\n        },\n        {\n          \"description\": \"Specifies the object identifier (OID) of the certificate policy under which the certificate was issued. For more information, see NIST's definition of <a href=\\\"https://csrc.nist.gov/glossary/term/Object_Identifier\\\">Object Identifier (OID)</a>.\"\n        }\n      ]\n    },\n    \"PolicyQualifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyQualifierInfoList\"\n\
  \        },\n        {\n          \"description\": \"Modifies the given <code>CertPolicyId</code> with a qualifier. Amazon Web Services Private CA supports the certification practice statement (CPS) qualifier.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertPolicyId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-policy-information-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: PolicyInformation
---
