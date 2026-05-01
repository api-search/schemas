---
description: Organization-wide EC2 instances with findings scan configuration.
layout: schema
name: OrganizationScanEc2InstanceWithFindings
properties_list:
- description: ''
  name: EbsVolumes
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-scan-ec2-instance-with-findings-schema.json
slug: guardduty-organization-scan-ec2-instance-with-findings
source_filename: guardduty-organization-scan-ec2-instance-with-findings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-scan-ec2-instance-with-findings-schema.json\",\n  \"title\": \"OrganizationScanEc2InstanceWithFindings\",\n  \"description\": \"Organization-wide EC2 instances with findings scan configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EbsVolumes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationEbsVolumes\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebsVolumes\"\n          },\n          \"description\": \"Whether scanning EBS volumes should be auto-enabled for new members joining the organization.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-scan-ec2-instance-with-findings-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationScanEc2InstanceWithFindings
---
