---
description: DescribeCertificateAuthorityAuditReportResponse schema from Amazon Private CA API
layout: schema
name: DescribeCertificateAuthorityAuditReportResponse
properties_list:
- description: ''
  name: AuditReportStatus
  type: object
- description: ''
  name: S3BucketName
  type: object
- description: ''
  name: S3Key
  type: object
- description: ''
  name: CreatedAt
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-describe-certificate-authority-audit-report-response-schema.json
slug: amazon-private-ca-describe-certificate-authority-audit-report-response
source_filename: amazon-private-ca-describe-certificate-authority-audit-report-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-describe-certificate-authority-audit-report-response-schema.json\",\n  \"title\": \"DescribeCertificateAuthorityAuditReportResponse\",\n  \"description\": \"DescribeCertificateAuthorityAuditReportResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuditReportStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditReportStatus\"\n        },\n        {\n          \"description\": \"Specifies whether report creation is in progress, has succeeded, or has failed.\"\n        }\n      ]\n    },\n    \"S3BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"Name of the S3 bucket that contains the report.\"\
  \n        }\n      ]\n    },\n    \"S3Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \"S3 <b>key</b> that uniquely identifies the report file in your S3 bucket.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date and time at which the report was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-describe-certificate-authority-audit-report-response-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: DescribeCertificateAuthorityAuditReportResponse
---
