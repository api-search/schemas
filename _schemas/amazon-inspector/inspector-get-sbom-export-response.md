---
description: GetSbomExportResponse schema
layout: schema
name: GetSbomExportResponse
properties_list:
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: filterCriteria
  type: object
- description: ''
  name: format
  type: object
- description: ''
  name: reportId
  type: object
- description: Contains details of the Amazon S3 bucket and KMS key used to export findings.
  name: s3Destination
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-get-sbom-export-response-schema.json
slug: inspector-get-sbom-export-response
source_filename: inspector-get-sbom-export-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-get-sbom-export-response-schema.json\",\n  \"title\": \"GetSbomExportResponse\",\n  \"description\": \"GetSbomExportResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportingErrorCode\"\n        },\n        {\n          \"description\": \"An error code.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"An error message.\"\n        }\n      ]\n    },\n    \"filterCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceFilterCriteria\"\n        },\n        {\n          \"description\": \"Contains\
  \ details about the resource filter criteria used for the software bill of materials (SBOM) report.\"\n        }\n      ]\n    },\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SbomReportFormat\"\n        },\n        {\n          \"description\": \"The format of the software bill of materials (SBOM) report.\"\n        }\n      ]\n    },\n    \"reportId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportId\"\n        },\n        {\n          \"description\": \"The report ID of the software bill of materials (SBOM) report.\"\n        }\n      ]\n    },\n    \"s3Destination\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"bucketName\",\n        \"kmsKeyArn\"\n      ],\n      \"properties\": {\n        \"bucketName\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/String\"\n            },\n            {\n              \"description\": \"The name of\
  \ the Amazon S3 bucket to export findings to.\"\n            }\n          ]\n        },\n        \"keyPrefix\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/String\"\n            },\n            {\n              \"description\": \"The prefix that the findings will be written under.\"\n            }\n          ]\n        },\n        \"kmsKeyArn\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/String\"\n            },\n            {\n              \"description\": \"The ARN of the KMS key used to encrypt data when exporting findings.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Contains details of the Amazon S3 bucket and KMS key used to export findings.\"\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalReportStatus\"\n        },\n        {\n          \"description\": \"The status of the software bill of materials\
  \ (SBOM) report.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-get-sbom-export-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: GetSbomExportResponse
---
