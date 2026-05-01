---
description: DescribeCertificateAuthorityAuditReportRequest schema from Amazon Private CA API
layout: schema
name: DescribeCertificateAuthorityAuditReportRequest
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: AuditReportId
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-describe-certificate-authority-audit-report-request-schema.json
slug: amazon-private-ca-describe-certificate-authority-audit-report-request
source_filename: amazon-private-ca-describe-certificate-authority-audit-report-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-describe-certificate-authority-audit-report-request-schema.json\",\n  \"title\": \"DescribeCertificateAuthorityAuditReportRequest\",\n  \"description\": \"DescribeCertificateAuthorityAuditReportRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the private CA. This must be of the form:</p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i> </code>. </p>\"\n        }\n      ]\n    },\n    \"AuditReportId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditReportId\"\
  \n        },\n        {\n          \"description\": \"The report ID returned by calling the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthorityAuditReport.html\\\">CreateCertificateAuthorityAuditReport</a> action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityArn\",\n    \"AuditReportId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-describe-certificate-authority-audit-report-request-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: DescribeCertificateAuthorityAuditReportRequest
---
