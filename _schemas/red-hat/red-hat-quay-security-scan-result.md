---
description: Security scan results for a container image manifest, including detected vulnerabilities.
layout: schema
name: SecurityScanResult
properties_list:
- description: The scan status.
  name: status
  type: string
- description: The scan result data.
  name: data
  type: object
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-quay-security-scan-result-schema.json
slug: red-hat-quay-security-scan-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityScanResult\",\n  \"type\": \"object\",\n  \"description\": \"Security scan results for a container image manifest, including detected vulnerabilities.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The scan status.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The scan result data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-quay-security-scan-result-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: SecurityScanResult
---
