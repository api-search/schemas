---
description: Modifies the <code>CertPolicyId</code> of a <code>PolicyInformation</code> object with a qualifier. Amazon Web Services Private CA supports the certification practice statement (CPS) qualifier.
layout: schema
name: PolicyQualifierInfo
properties_list:
- description: ''
  name: PolicyQualifierId
  type: object
- description: ''
  name: Qualifier
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-policy-qualifier-info-schema.json
slug: amazon-private-ca-policy-qualifier-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-policy-qualifier-info-schema.json\",\n  \"title\": \"PolicyQualifierInfo\",\n  \"description\": \"Modifies the <code>CertPolicyId</code> of a <code>PolicyInformation</code> object with a qualifier. Amazon Web Services Private CA supports the certification practice statement (CPS) qualifier.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyQualifierId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyQualifierId\"\n        },\n        {\n          \"description\": \"Identifies the qualifier modifying a <code>CertPolicyId</code>.\"\n        }\n      ]\n    },\n    \"Qualifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Qualifier\"\n        },\n        {\n          \"description\": \"Defines the qualifier\
  \ type. Amazon Web Services Private CA supports the use of a URI for a CPS qualifier in this field.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PolicyQualifierId\",\n    \"Qualifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-policy-qualifier-info-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: PolicyQualifierInfo
---
