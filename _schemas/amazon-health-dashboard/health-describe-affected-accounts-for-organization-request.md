---
description: DescribeAffectedAccountsForOrganizationRequest schema from Amazon Health Dashboard API
layout: schema
name: DescribeAffectedAccountsForOrganizationRequest
properties_list:
- description: ''
  name: eventArn
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-affected-accounts-for-organization-request-schema.json
slug: health-describe-affected-accounts-for-organization-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-affected-accounts-for-organization-request-schema.json\",\n  \"title\": \"DescribeAffectedAccountsForOrganizationRequest\",\n  \"description\": \"DescribeAffectedAccountsForOrganizationRequest schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventArn\"\n        },\n        {\n          \"description\": \"<p>The unique identifier for the event. The event ARN has the <code>arn:aws:health:<i>event-region</i>::event/<i>SERVICE</i>/<i>EVENT_TYPE_CODE</i>/<i>EVENT_TYPE_PLUS_ID</i> </code> format.</p> <p>For example, an event ARN might look like the following:</p> <p> <code>arn:aws:health:us-east-1::event/EC2/EC2_INSTANCE_RETIREMENT_SCHEDULED/EC2_INSTANCE_RETIREMENT_SCHEDULED_ABC123-DEF456</code>\
  \ </p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \"If the results of a search are large, only a portion of the results are returned, and a <code>nextToken</code> pagination token is returned in the response. To retrieve the next batch of results, reissue the search request and include the returned token. When all results have been returned, the response does not contain a pagination token value.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/maxResults\"\n        },\n        {\n          \"description\": \"The maximum number of items to return in one batch, between 10 and 100, inclusive.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-affected-accounts-for-organization-request-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeAffectedAccountsForOrganizationRequest
---
