---
description: DescribeEventDetailsForOrganizationRequest schema from Amazon Health Dashboard API
layout: schema
name: DescribeEventDetailsForOrganizationRequest
properties_list:
- description: ''
  name: organizationEventDetailFilters
  type: object
- description: ''
  name: locale
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-event-details-for-organization-request-schema.json
slug: health-describe-event-details-for-organization-request
source_filename: health-describe-event-details-for-organization-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-event-details-for-organization-request-schema.json\",\n  \"title\": \"DescribeEventDetailsForOrganizationRequest\",\n  \"description\": \"DescribeEventDetailsForOrganizationRequest schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organizationEventDetailFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationEventDetailFiltersList\"\n        },\n        {\n          \"description\": \"A set of JSON elements that includes the <code>awsAccountId</code> and the <code>eventArn</code>.\"\n        }\n      ]\n    },\n    \"locale\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/locale\"\n        },\n        {\n          \"description\": \"The locale (language) to return\
  \ information in. English (en) is the default and the only supported value at this time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"organizationEventDetailFilters\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-event-details-for-organization-request-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeEventDetailsForOrganizationRequest
---
