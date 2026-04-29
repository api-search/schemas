---
description: Represents an ACM SSL/TLS certificate with its associated metadata, domain validation, and lifecycle information.
layout: schema
name: Amazon Certificate Manager Certificate
properties_list:
- description: The Amazon Resource Name (ARN) of the certificate.
  name: certificateArn
  type: string
- description: The fully qualified domain name for the certificate.
  name: domainName
  type: string
- description: One or more domain names (subject alternative names) included in the certificate.
  name: subjectAlternativeNames
  type: array
- description: The status of the certificate.
  name: status
  type: string
- description: The source of the certificate.
  name: type
  type: string
- description: The name of the certificate authority that issued the certificate.
  name: issuer
  type: string
- description: The serial number of the certificate.
  name: serial
  type: string
- description: The algorithm used to generate the key pair.
  name: keyAlgorithm
  type: string
- description: The time at which the certificate was requested.
  name: createdAt
  type: string
- description: The time at which the certificate was issued.
  name: issuedAt
  type: string
- description: The time before which the certificate is not valid.
  name: notBefore
  type: string
- description: The time after which the certificate is not valid.
  name: notAfter
  type: string
- description: Whether the certificate is eligible for renewal.
  name: renewalEligibility
  type: string
provider_name: Amazon Certificate Manager
provider_slug: amazon-certificate-manager
schema_file: json-schema/amazon-certificate-manager-certificate-schema.json
slug: amazon-certificate-manager-certificate
source_filename: amazon-certificate-manager-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/acm/certificate.json\",\n  \"title\": \"Amazon Certificate Manager Certificate\",\n  \"description\": \"Represents an ACM SSL/TLS certificate with its associated metadata, domain validation, and lifecycle information.\",\n  \"type\": \"object\",\n  \"required\": [\"certificateArn\", \"domainName\"],\n  \"properties\": {\n    \"certificateArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the certificate.\",\n      \"pattern\": \"^arn:aws:acm:[a-z0-9-]+:[0-9]{12}:certificate/.+$\"\n    },\n    \"domainName\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified domain name for the certificate.\"\n    },\n    \"subjectAlternativeNames\": {\n      \"type\": \"array\",\n      \"description\": \"One or more domain names (subject alternative names) included in the certificate.\",\n      \"\
  items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the certificate.\",\n      \"enum\": [\n        \"PENDING_VALIDATION\",\n        \"ISSUED\",\n        \"INACTIVE\",\n        \"REVOKED\",\n        \"EXPIRED\",\n        \"VALIDATION_TIMED_OUT\",\n        \"FAILED\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The source of the certificate.\",\n      \"enum\": [\n        \"IMPORTED\",\n        \"AMAZON_ISSUED\",\n        \"PRIVATE\"\n      ]\n    },\n    \"issuer\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the certificate authority that issued the certificate.\"\n    },\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"The serial number of the certificate.\"\n    },\n    \"keyAlgorithm\": {\n      \"type\": \"string\",\n      \"description\": \"The algorithm used to generate the key pair.\",\n     \
  \ \"enum\": [\n        \"RSA_1024\",\n        \"RSA_2048\",\n        \"RSA_3072\",\n        \"RSA_4096\",\n        \"EC_prime256v1\",\n        \"EC_secp384r1\",\n        \"EC_secp521r1\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time at which the certificate was requested.\"\n    },\n    \"issuedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time at which the certificate was issued.\"\n    },\n    \"notBefore\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time before which the certificate is not valid.\"\n    },\n    \"notAfter\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time after which the certificate is not valid.\"\n    },\n    \"renewalEligibility\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the certificate is eligible\
  \ for renewal.\",\n      \"enum\": [\n        \"ELIGIBLE\",\n        \"INELIGIBLE\"\n      ]\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-certificate-manager/refs/heads/main/json-schema/amazon-certificate-manager-certificate-schema.json
tags:
- AWS
- Certificates
- Encryption
- Security
- SSL
- TLS
title: Amazon Certificate Manager Certificate
---
