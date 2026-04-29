---
description: RelationshipStatus schema
layout: schema
name: RelationshipStatus
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-relationship-status-schema.json
slug: inspector-relationship-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-relationship-status-schema.json\",\n  \"title\": \"RelationshipStatus\",\n  \"description\": \"RelationshipStatus schema\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CREATED\",\n    \"INVITED\",\n    \"DISABLED\",\n    \"ENABLED\",\n    \"REMOVED\",\n    \"RESIGNED\",\n    \"DELETED\",\n    \"EMAIL_VERIFICATION_IN_PROGRESS\",\n    \"EMAIL_VERIFICATION_FAILED\",\n    \"REGION_DISABLED\",\n    \"ACCOUNT_SUSPENDED\",\n    \"CANNOT_CREATE_DETECTOR_IN_ORG_MASTER\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-relationship-status-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: RelationshipStatus
---
