---
description: UpdateEnrollmentStatusRequest schema
layout: schema
name: UpdateEnrollmentStatusRequest
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: includeMemberAccounts
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-update-enrollment-status-request-schema.json
slug: compute-optimizer-update-enrollment-status-request
source_filename: compute-optimizer-update-enrollment-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-update-enrollment-status-request-schema.json\",\n  \"title\": \"UpdateEnrollmentStatusRequest\",\n  \"description\": \"UpdateEnrollmentStatusRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"<p>The new enrollment status of the account.</p> <p>The following status options are available:</p> <ul> <li> <p> <code>Active</code> - Opts in your account to the Compute Optimizer service. Compute Optimizer begins analyzing the configuration and utilization metrics of your Amazon Web Services resources after you opt in. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/metrics.html\\\
  \">Metrics analyzed by Compute Optimizer</a> in the <i>Compute Optimizer User Guide</i>.</p> </li> <li> <p> <code>Inactive</code> - Opts out your account from the Compute Optimizer service. Your account's recommendations and related metrics data will be deleted from Compute Optimizer after you opt out.</p> </li> </ul> <note> <p>The <code>Pending</code> and <code>Failed</code> options cannot be used to update the enrollment status of an account. They are returned in the response of a request to update the enrollment status of an account.</p> </note>\"\n        }\n      ]\n    },\n    \"includeMemberAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncludeMemberAccounts\"\n        },\n        {\n          \"description\": \"Indicates whether to enroll member accounts of the organization if the account is the management account of an organization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-update-enrollment-status-request-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: UpdateEnrollmentStatusRequest
---
