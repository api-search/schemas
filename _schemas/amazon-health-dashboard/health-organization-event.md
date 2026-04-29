---
description: Summary information about an event, returned by the <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventsForOrganization.html">DescribeEventsForOrganization</a> operation.
layout: schema
name: OrganizationEvent
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: service
  type: object
- description: ''
  name: eventTypeCode
  type: object
- description: ''
  name: eventTypeCategory
  type: object
- description: ''
  name: eventScopeCode
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: lastUpdatedTime
  type: object
- description: ''
  name: statusCode
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-organization-event-schema.json
slug: health-organization-event
source_filename: health-organization-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-organization-event-schema.json\",\n  \"title\": \"OrganizationEvent\",\n  \"description\": \"Summary information about an event, returned by the <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventsForOrganization.html\\\">DescribeEventsForOrganization</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventArn\"\n        },\n        {\n          \"description\": \"<p>The unique identifier for the event. The event ARN has the <code>arn:aws:health:<i>event-region</i>::event/<i>SERVICE</i>/<i>EVENT_TYPE_CODE</i>/<i>EVENT_TYPE_PLUS_ID</i> </code> format.</p> <p>For example, an event ARN might look like the following:</p> <p> <code>arn:aws:health:us-east-1::event/EC2/EC2_INSTANCE_RETIREMENT_SCHEDULED/EC2_INSTANCE_RETIREMENT_SCHEDULED_ABC123-DEF456</code>\
  \ </p>\"\n        }\n      ]\n    },\n    \"service\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/service\"\n        },\n        {\n          \"description\": \"The Amazon Web Services service that is affected by the event, such as EC2 and RDS.\"\n        }\n      ]\n    },\n    \"eventTypeCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventTypeCode\"\n        },\n        {\n          \"description\": \"The unique identifier for the event type. The format is <code>AWS_SERVICE_DESCRIPTION</code>. For example, <code>AWS_EC2_SYSTEM_MAINTENANCE_EVENT</code>.\"\n        }\n      ]\n    },\n    \"eventTypeCategory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventTypeCategory\"\n        },\n        {\n          \"description\": \"A list of event type category codes. Possible values are <code>issue</code>, <code>accountNotification</code>, or <code>scheduledChange</code>. Currently, the\
  \ <code>investigation</code> value isn't supported at this time.\"\n        }\n      ]\n    },\n    \"eventScopeCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventScopeCode\"\n        },\n        {\n          \"description\": \"<p>This parameter specifies if the Health event is a public Amazon Web Services service event or an account-specific event.</p> <ul> <li> <p>If the <code>eventScopeCode</code> value is <code>PUBLIC</code>, then the <code>affectedAccounts</code> value is always empty.</p> </li> <li> <p>If the <code>eventScopeCode</code> value is <code>ACCOUNT_SPECIFIC</code>, then the <code>affectedAccounts</code> value lists the affected Amazon Web Services accounts in your organization. For example, if an event affects a service such as Amazon Elastic Compute Cloud and you have Amazon Web Services accounts that use that service, those account IDs appear in the response.</p> </li> <li> <p>If the <code>eventScopeCode</code> value is <code>NONE</code>,\
  \ then the <code>eventArn</code> that you specified in the request is invalid or doesn't exist.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/region\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region name of the event.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the event began.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the event ended.\"\n        }\n      ]\n    },\n    \"lastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\"\
  : \"The most recent date and time that the event was updated.\"\n        }\n      ]\n    },\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventStatusCode\"\n        },\n        {\n          \"description\": \"The most recent status of the event. Possible values are <code>open</code>, <code>closed</code>, and <code>upcoming</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-organization-event-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: OrganizationEvent
---
