---
description: GetEnrollmentStatusResponse schema
layout: schema
name: GetEnrollmentStatusResponse
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
- description: ''
  name: memberAccountsEnrolled
  type: object
- description: ''
  name: lastUpdatedTimestamp
  type: object
- description: ''
  name: numberOfMemberAccountsOptedIn
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-enrollment-status-response-schema.json
slug: compute-optimizer-get-enrollment-status-response
source_filename: compute-optimizer-get-enrollment-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-enrollment-status-response-schema.json\",\n  \"title\": \"GetEnrollmentStatusResponse\",\n  \"description\": \"GetEnrollmentStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The enrollment status of the account.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusReason\"\n        },\n        {\n          \"description\": \"<p>The reason for the enrollment status of the account.</p> <p>For example, an account might show a status of <code>Pending</code> because member accounts of an organization require more time to\
  \ be enrolled in the service.</p>\"\n        }\n      ]\n    },\n    \"memberAccountsEnrolled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberAccountsEnrolled\"\n        },\n        {\n          \"description\": \"Confirms the enrollment status of member accounts of the organization, if the account is a management account of an organization.\"\n        }\n      ]\n    },\n    \"lastUpdatedTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedTimestamp\"\n        },\n        {\n          \"description\": \"The Unix epoch timestamp, in seconds, of when the account enrollment status was last updated.\"\n        }\n      ]\n    },\n    \"numberOfMemberAccountsOptedIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberOfMemberAccountsOptedIn\"\n        },\n        {\n          \"description\": \"The count of organization member accounts that are opted in to the service, if\
  \ your account is an organization management account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-enrollment-status-response-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetEnrollmentStatusResponse
---
