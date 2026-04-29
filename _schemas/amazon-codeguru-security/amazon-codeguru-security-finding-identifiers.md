---
description: FindingIdentifiers schema from Amazon CodeGuru Security
layout: schema
name: FindingIdentifiers
properties_list: []
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-finding-identifiers-schema.json
slug: amazon-codeguru-security-finding-identifiers
source_filename: amazon-codeguru-security-finding-identifiers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-finding-identifiers-schema.json\",\n  \"title\": \"FindingIdentifiers\",\n  \"description\": \"FindingIdentifiers schema from Amazon CodeGuru Security\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/FindingIdentifier\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 25\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-finding-identifiers-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: FindingIdentifiers
---
