---
description: DescribeAffectedEntitiesForOrganizationResponse schema from Amazon Health Dashboard API
layout: schema
name: DescribeAffectedEntitiesForOrganizationResponse
properties_list:
- description: ''
  name: entities
  type: object
- description: ''
  name: failedSet
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-affected-entities-for-organization-response-schema.json
slug: health-describe-affected-entities-for-organization-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-affected-entities-for-organization-response-schema.json\",\n  \"title\": \"DescribeAffectedEntitiesForOrganizationResponse\",\n  \"description\": \"DescribeAffectedEntitiesForOrganizationResponse schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityList\"\n        },\n        {\n          \"description\": \"A JSON set of elements including the <code>awsAccountId</code> and its <code>entityArn</code>, <code>entityValue</code> and its <code>entityArn</code>, <code>lastUpdatedTime</code>, and <code>statusCode</code>.\"\n        }\n      ]\n    },\n    \"failedSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescribeAffectedEntitiesForOrganizationFailedSet\"\
  \n        },\n        {\n          \"description\": \"A JSON set of elements of the failed response, including the <code>awsAccountId</code>, <code>errorMessage</code>, <code>errorName</code>, and <code>eventArn</code>.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \"If the results of a search are large, only a portion of the results are returned, and a <code>nextToken</code> pagination token is returned in the response. To retrieve the next batch of results, reissue the search request and include the returned token. When all results have been returned, the response does not contain a pagination token value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-affected-entities-for-organization-response-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeAffectedEntitiesForOrganizationResponse
---
