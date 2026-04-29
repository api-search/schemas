---
description: CreateCertificateAuthorityAuditReportRequest schema from Amazon Private CA API
layout: schema
name: CreateCertificateAuthorityAuditReportRequest
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: S3BucketName
  type: object
- description: ''
  name: AuditReportResponseFormat
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-create-certificate-authority-audit-report-request-schema.json
slug: amazon-private-ca-create-certificate-authority-audit-report-request
source_filename: amazon-private-ca-create-certificate-authority-audit-report-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-create-certificate-authority-audit-report-request-schema.json\",\n  \"title\": \"CreateCertificateAuthorityAuditReportRequest\",\n  \"description\": \"CreateCertificateAuthorityAuditReportRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the CA to be audited. This is of the form:</p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i> </code>.</p>\"\n        }\n      ]\n    },\n    \"S3BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\
  \n        },\n        {\n          \"description\": \"The name of the S3 bucket that will contain the audit report.\"\n        }\n      ]\n    },\n    \"AuditReportResponseFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditReportResponseFormat\"\n        },\n        {\n          \"description\": \"The format in which to create the report. This can be either <b>JSON</b> or <b>CSV</b>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityArn\",\n    \"S3BucketName\",\n    \"AuditReportResponseFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-create-certificate-authority-audit-report-request-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: CreateCertificateAuthorityAuditReportRequest
---
