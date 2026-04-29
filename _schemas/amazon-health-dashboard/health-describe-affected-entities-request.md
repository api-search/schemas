---
description: DescribeAffectedEntitiesRequest schema from Amazon Health Dashboard API
layout: schema
name: DescribeAffectedEntitiesRequest
properties_list:
- description: ''
  name: filter
  type: object
- description: ''
  name: locale
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-affected-entities-request-schema.json
slug: health-describe-affected-entities-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-affected-entities-request-schema.json\",\n  \"title\": \"DescribeAffectedEntitiesRequest\",\n  \"description\": \"DescribeAffectedEntitiesRequest schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityFilter\"\n        },\n        {\n          \"description\": \"Values to narrow the results returned. At least one event ARN is required.\"\n        }\n      ]\n    },\n    \"locale\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/locale\"\n        },\n        {\n          \"description\": \"The locale (language) to return information in. English (en) is the default and the only supported value at this time.\"\n        }\n\
  \      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \"If the results of a search are large, only a portion of the results are returned, and a <code>nextToken</code> pagination token is returned in the response. To retrieve the next batch of results, reissue the search request and include the returned token. When all results have been returned, the response does not contain a pagination token value.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/maxResults\"\n        },\n        {\n          \"description\": \"The maximum number of items to return in one batch, between 10 and 100, inclusive.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"filter\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-affected-entities-request-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeAffectedEntitiesRequest
---
