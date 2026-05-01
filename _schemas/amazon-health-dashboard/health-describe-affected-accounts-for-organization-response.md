---
description: DescribeAffectedAccountsForOrganizationResponse schema from Amazon Health Dashboard API
layout: schema
name: DescribeAffectedAccountsForOrganizationResponse
properties_list:
- description: ''
  name: affectedAccounts
  type: object
- description: ''
  name: eventScopeCode
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-affected-accounts-for-organization-response-schema.json
slug: health-describe-affected-accounts-for-organization-response
source_filename: health-describe-affected-accounts-for-organization-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-affected-accounts-for-organization-response-schema.json\",\n  \"title\": \"DescribeAffectedAccountsForOrganizationResponse\",\n  \"description\": \"DescribeAffectedAccountsForOrganizationResponse schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"affectedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/affectedAccountsList\"\n        },\n        {\n          \"description\": \"A JSON set of elements of the affected accounts.\"\n        }\n      ]\n    },\n    \"eventScopeCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventScopeCode\"\n        },\n        {\n          \"description\": \"<p>This parameter specifies if the Health event is a public Amazon Web Services\
  \ service event or an account-specific event.</p> <ul> <li> <p>If the <code>eventScopeCode</code> value is <code>PUBLIC</code>, then the <code>affectedAccounts</code> value is always empty.</p> </li> <li> <p>If the <code>eventScopeCode</code> value is <code>ACCOUNT_SPECIFIC</code>, then the <code>affectedAccounts</code> value lists the affected Amazon Web Services accounts in your organization. For example, if an event affects a service such as Amazon Elastic Compute Cloud and you have Amazon Web Services accounts that use that service, those account IDs appear in the response.</p> </li> <li> <p>If the <code>eventScopeCode</code> value is <code>NONE</code>, then the <code>eventArn</code> that you specified in the request is invalid or doesn't exist.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \"If the results of a search are large,\
  \ only a portion of the results are returned, and a <code>nextToken</code> pagination token is returned in the response. To retrieve the next batch of results, reissue the search request and include the returned token. When all results have been returned, the response does not contain a pagination token value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-affected-accounts-for-organization-response-schema.json
tags:
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeAffectedAccountsForOrganizationResponse
---
