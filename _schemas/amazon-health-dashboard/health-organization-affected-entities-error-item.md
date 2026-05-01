---
description: Error information returned when a <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeAffectedEntitiesForOrganization.html">DescribeAffectedEntitiesForOrganization</a> operation can't find or process a specific entity.
layout: schema
name: OrganizationAffectedEntitiesErrorItem
properties_list:
- description: ''
  name: awsAccountId
  type: object
- description: ''
  name: eventArn
  type: object
- description: ''
  name: errorName
  type: object
- description: ''
  name: errorMessage
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-organization-affected-entities-error-item-schema.json
slug: health-organization-affected-entities-error-item
source_filename: health-organization-affected-entities-error-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-organization-affected-entities-error-item-schema.json\",\n  \"title\": \"OrganizationAffectedEntitiesErrorItem\",\n  \"description\": \"Error information returned when a <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeAffectedEntitiesForOrganization.html\\\">DescribeAffectedEntitiesForOrganization</a> operation can't find or process a specific entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/accountId\"\n        },\n        {\n          \"description\": \"The 12-digit Amazon Web Services account numbers that contains the affected entities.\"\n        }\n      ]\n    },\n    \"eventArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventArn\"\
  \n        },\n        {\n          \"description\": \"<p>The unique identifier for the event. The event ARN has the <code>arn:aws:health:<i>event-region</i>::event/<i>SERVICE</i>/<i>EVENT_TYPE_CODE</i>/<i>EVENT_TYPE_PLUS_ID</i> </code> format.</p> <p>For example, an event ARN might look like the following:</p> <p> <code>arn:aws:health:us-east-1::event/EC2/EC2_INSTANCE_RETIREMENT_SCHEDULED/EC2_INSTANCE_RETIREMENT_SCHEDULED_ABC123-DEF456</code> </p>\"\n        }\n      ]\n    },\n    \"errorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The name of the error.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The unique identifier for the event type. The format is <code>AWS_SERVICE_DESCRIPTION</code>. For example, <code>AWS_EC2_SYSTEM_MAINTENANCE_EVENT</code>.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-organization-affected-entities-error-item-schema.json
tags:
- Health Monitoring
- Notifications
- Operations
- Service Status
title: OrganizationAffectedEntitiesErrorItem
---
