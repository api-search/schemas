---
description: DescribeHealthServiceStatusForOrganizationResponse schema from Amazon Health Dashboard API
layout: schema
name: DescribeHealthServiceStatusForOrganizationResponse
properties_list:
- description: ''
  name: healthServiceAccessStatusForOrganization
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-health-service-status-for-organization-response-schema.json
slug: health-describe-health-service-status-for-organization-response
source_filename: health-describe-health-service-status-for-organization-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-health-service-status-for-organization-response-schema.json\",\n  \"title\": \"DescribeHealthServiceStatusForOrganizationResponse\",\n  \"description\": \"DescribeHealthServiceStatusForOrganizationResponse schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"healthServiceAccessStatusForOrganization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/healthServiceAccessStatusForOrganization\"\n        },\n        {\n          \"description\": \"<p>Information about the status of enabling or disabling the Health organizational view feature in your organization.</p> <p>Valid values are <code>ENABLED | DISABLED | PENDING</code>. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-health-service-status-for-organization-response-schema.json
tags:
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeHealthServiceStatusForOrganizationResponse
---
