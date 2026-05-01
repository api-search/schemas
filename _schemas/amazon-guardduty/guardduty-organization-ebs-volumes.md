---
description: Organization-wide EBS volumes scan configuration.
layout: schema
name: OrganizationEbsVolumes
properties_list:
- description: ''
  name: AutoEnable
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-ebs-volumes-schema.json
slug: guardduty-organization-ebs-volumes
source_filename: guardduty-organization-ebs-volumes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-ebs-volumes-schema.json\",\n  \"title\": \"OrganizationEbsVolumes\",\n  \"description\": \"Organization-wide EBS volumes scan configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"autoEnable\"\n          },\n          \"description\": \"Whether scanning EBS volumes should be auto-enabled for new members joining the organization.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-ebs-volumes-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationEbsVolumes
---
