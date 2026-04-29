---
description: DescribeEventDetailsRequest schema from Amazon Health Dashboard API
layout: schema
name: DescribeEventDetailsRequest
properties_list:
- description: ''
  name: eventArns
  type: object
- description: ''
  name: locale
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-event-details-request-schema.json
slug: health-describe-event-details-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-event-details-request-schema.json\",\n  \"title\": \"DescribeEventDetailsRequest\",\n  \"description\": \"DescribeEventDetailsRequest schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventArnList\"\n        },\n        {\n          \"description\": \"A list of event ARNs (unique identifiers). For example: <code>\\\"arn:aws:health:us-east-1::event/EC2/EC2_INSTANCE_RETIREMENT_SCHEDULED/EC2_INSTANCE_RETIREMENT_SCHEDULED_ABC123-CDE456\\\", \\\"arn:aws:health:us-west-1::event/EBS/AWS_EBS_LOST_VOLUME/AWS_EBS_LOST_VOLUME_CHI789_JKL101\\\"</code> \"\n        }\n      ]\n    },\n    \"locale\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/locale\"\
  \n        },\n        {\n          \"description\": \"The locale (language) to return information in. English (en) is the default and the only supported value at this time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventArns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-event-details-request-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeEventDetailsRequest
---
