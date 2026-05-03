---
description: Schema describing the result of a Clair vulnerability scan for a Quay manifest.
layout: schema
name: Quay Manifest Security Scan
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: data
  type: object
provider_name: Quay
provider_slug: quay
schema_file: json-schema/quay-manifest-security-schema.json
slug: quay-manifest-security
source_filename: quay-manifest-security-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/json-schema/quay-manifest-security-schema.json\",\n  \"title\": \"Quay Manifest Security Scan\",\n  \"description\": \"Schema describing the result of a Clair vulnerability scan for a Quay manifest.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"queued\", \"scanning\", \"scanned\", \"unsupported\", \"error\"]\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Layer\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Name\": {\n              \"type\": \"string\"\n            },\n            \"ParentName\": {\n              \"type\": \"string\"\n            },\n            \"NamespaceName\": {\n              \"type\": \"string\"\n            },\n            \"IndexedByVersion\": {\n       \
  \       \"type\": \"integer\"\n            },\n            \"Features\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"Name\": { \"type\": \"string\" },\n                  \"Version\": { \"type\": \"string\" },\n                  \"VersionFormat\": { \"type\": \"string\" },\n                  \"Vulnerabilities\": {\n                    \"type\": \"array\",\n                    \"items\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"Name\": { \"type\": \"string\" },\n                        \"NamespaceName\": { \"type\": \"string\" },\n                        \"Description\": { \"type\": \"string\" },\n                        \"Link\": { \"type\": \"string\", \"format\": \"uri\" },\n                        \"Severity\": {\n                          \"type\": \"string\",\n                          \"enum\"\
  : [\"Unknown\", \"Negligible\", \"Low\", \"Medium\", \"High\", \"Critical\", \"Defcon1\"]\n                        },\n                        \"FixedBy\": { \"type\": \"string\" }\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/json-schema/quay-manifest-security-schema.json
tags:
- Container Images
- Containers
- Red Hat
- Registry
- Security Scanning
title: Quay Manifest Security Scan
---
