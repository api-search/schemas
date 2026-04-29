---
description: CreateCertificateAuthorityAuditReportResponse schema from Amazon Private CA API
layout: schema
name: CreateCertificateAuthorityAuditReportResponse
properties_list:
- description: ''
  name: AuditReportId
  type: object
- description: ''
  name: S3Key
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-create-certificate-authority-audit-report-response-schema.json
slug: amazon-private-ca-create-certificate-authority-audit-report-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-create-certificate-authority-audit-report-response-schema.json\",\n  \"title\": \"CreateCertificateAuthorityAuditReportResponse\",\n  \"description\": \"CreateCertificateAuthorityAuditReportResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuditReportId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditReportId\"\n        },\n        {\n          \"description\": \"An alphanumeric string that contains a report identifier.\"\n        }\n      ]\n    },\n    \"S3Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \"The <b>key</b> that uniquely identifies the report file in your S3 bucket.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-create-certificate-authority-audit-report-response-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: CreateCertificateAuthorityAuditReportResponse
---
