---
description: RequestCertificateRequest schema from Amazon Certificate Manager API
layout: schema
name: RequestCertificateRequest
properties_list:
- description: The fully qualified domain name for the certificate.
  name: DomainName
  type: string
- description: Additional FQDNs to be included in the certificate.
  name: SubjectAlternativeNames
  type: array
- description: The method to use for validation.
  name: ValidationMethod
  type: string
- description: Token to prevent duplicate requests.
  name: IdempotencyToken
  type: string
provider_name: Amazon Certificate Manager
provider_slug: amazon-certificate-manager
schema_file: json-schema/certificate-manager-request-certificate-request-schema.json
slug: certificate-manager-request-certificate-request
source_filename: certificate-manager-request-certificate-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-certificate-manager/refs/heads/main/json-schema/certificate-manager-request-certificate-request-schema.json\",\n  \"title\": \"RequestCertificateRequest\",\n  \"description\": \"RequestCertificateRequest schema from Amazon Certificate Manager API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified domain name for the certificate.\"\n    },\n    \"SubjectAlternativeNames\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional FQDNs to be included in the certificate.\"\n    },\n    \"ValidationMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"EMAIL\",\n        \"DNS\"\n      ],\n      \"description\": \"The method to use for validation.\"\n    },\n    \"\
  IdempotencyToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token to prevent duplicate requests.\"\n    }\n  },\n  \"required\": [\n    \"DomainName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-certificate-manager/refs/heads/main/json-schema/certificate-manager-request-certificate-request-schema.json
tags:
- AWS
- Certificates
- Encryption
- Security
- SSL
- TLS
title: RequestCertificateRequest
---
