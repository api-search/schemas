---
description: Contains information about the domain.
layout: schema
name: DomainDetails
properties_list:
- description: ''
  name: Domain
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-domain-details-schema.json
slug: guardduty-domain-details
source_filename: guardduty-domain-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-domain-details-schema.json\",\n  \"title\": \"DomainDetails\",\n  \"description\": \"Contains information about the domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"domain\"\n          },\n          \"description\": \"The domain information for the Amazon Web Services API call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-domain-details-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DomainDetails
---
