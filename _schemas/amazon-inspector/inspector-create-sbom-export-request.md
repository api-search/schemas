---
description: CreateSbomExportRequest schema
layout: schema
name: CreateSbomExportRequest
properties_list:
- description: ''
  name: reportFormat
  type: object
- description: ''
  name: resourceFilterCriteria
  type: object
- description: Contains details of the Amazon S3 bucket and KMS key used to export findings.
  name: s3Destination
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-create-sbom-export-request-schema.json
slug: inspector-create-sbom-export-request
source_filename: inspector-create-sbom-export-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-create-sbom-export-request-schema.json\",\n  \"title\": \"CreateSbomExportRequest\",\n  \"description\": \"CreateSbomExportRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SbomReportFormat\"\n        },\n        {\n          \"description\": \"The output format for the software bill of materials (SBOM) report.\"\n        }\n      ]\n    },\n    \"resourceFilterCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceFilterCriteria\"\n        },\n        {\n          \"description\": \"The resource filter criteria for the software bill of materials (SBOM) report.\"\n        }\n      ]\n    },\n    \"s3Destination\": {\n      \"type\": \"object\"\
  ,\n      \"required\": [\n        \"bucketName\",\n        \"kmsKeyArn\"\n      ],\n      \"properties\": {\n        \"bucketName\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/String\"\n            },\n            {\n              \"description\": \"The name of the Amazon S3 bucket to export findings to.\"\n            }\n          ]\n        },\n        \"keyPrefix\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/String\"\n            },\n            {\n              \"description\": \"The prefix that the findings will be written under.\"\n            }\n          ]\n        },\n        \"kmsKeyArn\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/String\"\n            },\n            {\n              \"description\": \"The ARN of the KMS key used to encrypt data when exporting findings.\"\n            }\n          ]\n        }\n      },\n      \"description\"\
  : \"Contains details of the Amazon S3 bucket and KMS key used to export findings.\"\n    }\n  },\n  \"required\": [\n    \"reportFormat\",\n    \"s3Destination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-create-sbom-export-request-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CreateSbomExportRequest
---
