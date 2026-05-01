---
description: 'The current status of the relationship between an account and an associated Amazon Macie administrator account. Possible values are:'
layout: schema
name: RelationshipStatus
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-relationship-status-schema.json
slug: amazon-macie-relationship-status
source_filename: amazon-macie-relationship-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-relationship-status-schema.json\",\n  \"title\": \"RelationshipStatus\",\n  \"description\": \"The current status of the relationship between an account and an associated Amazon Macie administrator account. Possible values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Enabled\",\n    \"Paused\",\n    \"Invited\",\n    \"Created\",\n    \"Removed\",\n    \"Resigned\",\n    \"EmailVerificationInProgress\",\n    \"EmailVerificationFailed\",\n    \"RegionDisabled\",\n    \"AccountSuspended\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-relationship-status-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: RelationshipStatus
---
