---
description: DescribeCertificateResponse schema from Amazon Certificate Manager API
layout: schema
name: DescribeCertificateResponse
properties_list:
- description: ''
  name: Certificate
  type: object
provider_name: Amazon Certificate Manager
provider_slug: amazon-certificate-manager
schema_file: json-schema/certificate-manager-describe-certificate-response-schema.json
slug: certificate-manager-describe-certificate-response
source_filename: certificate-manager-describe-certificate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-certificate-manager/refs/heads/main/json-schema/certificate-manager-describe-certificate-response-schema.json\",\n  \"title\": \"DescribeCertificateResponse\",\n  \"description\": \"DescribeCertificateResponse schema from Amazon Certificate Manager API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Certificate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"CertificateArn\": {\n          \"type\": \"string\"\n        },\n        \"DomainName\": {\n          \"type\": \"string\"\n        },\n        \"SubjectAlternativeNames\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"Status\": {\n          \"type\": \"string\"\n        },\n        \"Type\": {\n          \"type\": \"string\"\n        },\n        \"Issuer\": {\n          \"\
  type\": \"string\"\n        },\n        \"CreatedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"IssuedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"NotBefore\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"NotAfter\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"Serial\": {\n          \"type\": \"string\"\n        },\n        \"KeyAlgorithm\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-certificate-manager/refs/heads/main/json-schema/certificate-manager-describe-certificate-response-schema.json
tags:
- Certificates
- Encryption
- Security
- SSL
- TLS
title: DescribeCertificateResponse
---
