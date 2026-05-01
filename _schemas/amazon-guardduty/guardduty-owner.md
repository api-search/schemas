---
description: Contains information on the owner of the bucket.
layout: schema
name: Owner
properties_list:
- description: ''
  name: Id
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-owner-schema.json
slug: guardduty-owner
source_filename: guardduty-owner-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-owner-schema.json\",\n  \"title\": \"Owner\",\n  \"description\": \"Contains information on the owner of the bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The canonical user ID of the bucket owner. For information about locating your canonical user ID see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/acct-identifiers.html#FindingCanonicalId\\\">Finding Your Account Canonical User ID.</a> \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-owner-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Owner
---
