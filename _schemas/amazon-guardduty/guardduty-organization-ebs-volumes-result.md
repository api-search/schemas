---
description: An object that contains information on the status of whether EBS volumes scanning will be enabled as a data source for an organization.
layout: schema
name: OrganizationEbsVolumesResult
properties_list:
- description: ''
  name: AutoEnable
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-ebs-volumes-result-schema.json
slug: guardduty-organization-ebs-volumes-result
source_filename: guardduty-organization-ebs-volumes-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-ebs-volumes-result-schema.json\",\n  \"title\": \"OrganizationEbsVolumesResult\",\n  \"description\": \"An object that contains information on the status of whether EBS volumes scanning will be enabled as a data source for an organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"autoEnable\"\n          },\n          \"description\": \"An object that contains the status of whether scanning EBS volumes should be auto-enabled for new members joining the organization.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-ebs-volumes-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationEbsVolumesResult
---
