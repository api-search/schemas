---
description: ScansWithMostOpenCriticalFindings schema from Amazon CodeGuru Security
layout: schema
name: ScansWithMostOpenCriticalFindings
properties_list: []
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-scans-with-most-open-critical-findings-schema.json
slug: amazon-codeguru-security-scans-with-most-open-critical-findings
source_filename: amazon-codeguru-security-scans-with-most-open-critical-findings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-scans-with-most-open-critical-findings-schema.json\",\n  \"title\": \"ScansWithMostOpenCriticalFindings\",\n  \"description\": \"ScansWithMostOpenCriticalFindings schema from Amazon CodeGuru Security\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ScanNameWithFindingNum\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 3\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-scans-with-most-open-critical-findings-schema.json
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: ScansWithMostOpenCriticalFindings
---
