---
description: The SSL certificate that can be used to encrypt connections between the endpoints and the replication instance.
layout: schema
name: Certificate
properties_list:
- description: ''
  name: CertificateIdentifier
  type: object
- description: ''
  name: CertificateCreationDate
  type: object
- description: ''
  name: CertificatePem
  type: object
- description: ''
  name: CertificateWallet
  type: object
- description: ''
  name: CertificateArn
  type: object
- description: ''
  name: CertificateOwner
  type: object
- description: ''
  name: ValidFromDate
  type: object
- description: ''
  name: ValidToDate
  type: object
- description: ''
  name: SigningAlgorithm
  type: object
- description: ''
  name: KeyLength
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-certificate-schema.json
slug: amazon-dms-certificate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-certificate-schema.json\",\n  \"title\": \"Certificate\",\n  \"description\": \"The SSL certificate that can be used to encrypt connections between the endpoints and the replication instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A customer-assigned name for the certificate. Identifiers must begin with a letter and must contain only ASCII letters, digits, and hyphens. They can't end with a hyphen or contain two consecutive hyphens.\"\n        }\n      ]\n    },\n    \"CertificateCreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\"\
  : \"The date that the certificate was created.\"\n        }\n      ]\n    },\n    \"CertificatePem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The contents of a <code>.pem</code> file, which contains an X.509 certificate.\"\n        }\n      ]\n    },\n    \"CertificateWallet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateWallet\"\n        },\n        {\n          \"description\": \"The location of an imported Oracle Wallet certificate for use with SSL. Example: <code>filebase64(\\\"${path.root}/rds-ca-2019-root.sso\\\")</code> \"\n        }\n      ]\n    },\n    \"CertificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the certificate.\"\n        }\n      ]\n    },\n    \"CertificateOwner\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The owner of the certificate.\"\n        }\n      ]\n    },\n    \"ValidFromDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The beginning date that the certificate is valid.\"\n        }\n      ]\n    },\n    \"ValidToDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The final date that the certificate is valid.\"\n        }\n      ]\n    },\n    \"SigningAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The signing algorithm for the certificate.\"\n        }\n      ]\n    },\n    \"KeyLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerOptional\"\
  \n        },\n        {\n          \"description\": \"The key length of the cryptographic algorithm being used.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-certificate-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: Certificate
---
