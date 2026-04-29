---
description: ListCertificatesResponse schema from Amazon Certificate Manager API
layout: schema
name: ListCertificatesResponse
properties_list:
- description: ''
  name: CertificateSummaryList
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Certificate Manager
provider_slug: amazon-certificate-manager
schema_file: json-schema/certificate-manager-list-certificates-response-schema.json
slug: certificate-manager-list-certificates-response
source_filename: certificate-manager-list-certificates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-certificate-manager/refs/heads/main/json-schema/certificate-manager-list-certificates-response-schema.json\",\n  \"title\": \"ListCertificatesResponse\",\n  \"description\": \"ListCertificatesResponse schema from Amazon Certificate Manager API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateSummaryList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"CertificateArn\": {\n            \"type\": \"string\"\n          },\n          \"DomainName\": {\n            \"type\": \"string\"\n          },\n          \"Status\": {\n            \"type\": \"string\"\n          },\n          \"Type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-certificate-manager/refs/heads/main/json-schema/certificate-manager-list-certificates-response-schema.json
tags:
- AWS
- Certificates
- Encryption
- Security
- SSL
- TLS
title: ListCertificatesResponse
---
