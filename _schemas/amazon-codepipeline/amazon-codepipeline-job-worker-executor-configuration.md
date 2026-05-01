---
description: Details about the polling configuration for the <code>JobWorker</code> action engine, or executor.
layout: schema
name: JobWorkerExecutorConfiguration
properties_list:
- description: ''
  name: pollingAccounts
  type: object
- description: ''
  name: pollingServicePrincipals
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-job-worker-executor-configuration-schema.json
slug: amazon-codepipeline-job-worker-executor-configuration
source_filename: amazon-codepipeline-job-worker-executor-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-job-worker-executor-configuration-schema.json\",\n  \"title\": \"JobWorkerExecutorConfiguration\",\n  \"description\": \"Details about the polling configuration for the <code>JobWorker</code> action engine, or executor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pollingAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PollingAccountList\"\n        },\n        {\n          \"description\": \"The accounts in which the job worker is configured and might poll for jobs as part of the action execution.\"\n        }\n      ]\n    },\n    \"pollingServicePrincipals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PollingServicePrincipalList\"\n        },\n        {\n          \"description\": \"The service\
  \ Principals in which the job worker is configured and might poll for jobs as part of the action execution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-job-worker-executor-configuration-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: JobWorkerExecutorConfiguration
---
