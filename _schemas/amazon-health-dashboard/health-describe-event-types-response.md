---
description: DescribeEventTypesResponse schema from Amazon Health Dashboard API
layout: schema
name: DescribeEventTypesResponse
properties_list:
- description: ''
  name: eventTypes
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-event-types-response-schema.json
slug: health-describe-event-types-response
source_filename: health-describe-event-types-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-event-types-response-schema.json\",\n  \"title\": \"DescribeEventTypesResponse\",\n  \"description\": \"DescribeEventTypesResponse schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventTypeList\"\n        },\n        {\n          \"description\": \"A list of event types that match the filter criteria. Event types have a category (<code>issue</code>, <code>accountNotification</code>, or <code>scheduledChange</code>), a service (for example, <code>EC2</code>, <code>RDS</code>, <code>DATAPIPELINE</code>, <code>BILLING</code>), and a code (in the format <code>AWS_<i>SERVICE</i>_<i>DESCRIPTION</i> </code>; for example, <code>AWS_EC2_SYSTEM_MAINTENANCE_EVENT</code>).\"\
  \n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \"If the results of a search are large, only a portion of the results are returned, and a <code>nextToken</code> pagination token is returned in the response. To retrieve the next batch of results, reissue the search request and include the returned token. When all results have been returned, the response does not contain a pagination token value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-event-types-response-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeEventTypesResponse
---
