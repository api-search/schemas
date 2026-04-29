---
description: VulnIdList schema
layout: schema
name: VulnIdList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-vuln-id-list-schema.json
slug: inspector-vuln-id-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-vuln-id-list-schema.json\",\n  \"title\": \"VulnIdList\",\n  \"description\": \"VulnIdList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^CVE-[12][0-9]{3}-[0-9]{1,10}$\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-vuln-id-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: VulnIdList
---
