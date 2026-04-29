---
description: <p/>
layout: schema
name: PutEvaluationsRequest
properties_list:
- description: ''
  name: Evaluations
  type: object
- description: ''
  name: ResultToken
  type: object
- description: ''
  name: TestMode
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-evaluations-request-schema.json
slug: config-put-evaluations-request
source_filename: config-put-evaluations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-evaluations-request-schema.json\",\n  \"title\": \"PutEvaluationsRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Evaluations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Evaluations\"\n        },\n        {\n          \"description\": \"The assessments that the Lambda function performs. Each evaluation identifies an Amazon Web Services resource and indicates whether it complies with the Config rule that invokes the Lambda function.\"\n        }\n      ]\n    },\n    \"ResultToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An encrypted token that associates an evaluation with an Config rule. Identifies the rule and the\
  \ event that triggered the evaluation.\"\n        }\n      ]\n    },\n    \"TestMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Use this parameter to specify a test run for <code>PutEvaluations</code>. You can verify whether your Lambda function will deliver evaluation results to Config. No updates occur to your existing evaluations, and evaluation results are not sent to Config.</p> <note> <p>When <code>TestMode</code> is <code>true</code>, <code>PutEvaluations</code> doesn't require a valid value for the <code>ResultToken</code> parameter, but the value cannot be null.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResultToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-evaluations-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutEvaluationsRequest
---
