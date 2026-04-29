---
description: The values used to filter results from the <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventDetailsForOrganization.html">DescribeEventDetailsForOrganization</a> and <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeAffectedEntitiesForOrganization.html">DescribeAffectedEntitiesForOrganization</a> operations.
layout: schema
name: EventAccountFilter
properties_list:
- description: ''
  name: eventArn
  type: object
- description: ''
  name: awsAccountId
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-event-account-filter-schema.json
slug: health-event-account-filter
source_filename: health-event-account-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-account-filter-schema.json\",\n  \"title\": \"EventAccountFilter\",\n  \"description\": \"The values used to filter results from the <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventDetailsForOrganization.html\\\">DescribeEventDetailsForOrganization</a> and <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeAffectedEntitiesForOrganization.html\\\">DescribeAffectedEntitiesForOrganization</a> operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventArn\"\n        },\n        {\n          \"description\": \"<p>The unique identifier for the event. The event ARN has the <code>arn:aws:health:<i>event-region</i>::event/<i>SERVICE</i>/<i>EVENT_TYPE_CODE</i>/<i>EVENT_TYPE_PLUS_ID</i>\
  \ </code> format.</p> <p>For example, an event ARN might look like the following:</p> <p> <code>arn:aws:health:us-east-1::event/EC2/EC2_INSTANCE_RETIREMENT_SCHEDULED/EC2_INSTANCE_RETIREMENT_SCHEDULED_ABC123-DEF456</code> </p>\"\n        }\n      ]\n    },\n    \"awsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/accountId\"\n        },\n        {\n          \"description\": \"The 12-digit Amazon Web Services account numbers that contains the affected entities.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-account-filter-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: EventAccountFilter
---
