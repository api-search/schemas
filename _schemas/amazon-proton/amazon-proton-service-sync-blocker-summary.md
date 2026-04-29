---
description: <p>If a service instance is manually updated, Proton wants to prevent accidentally overriding a manual change.</p> <p>A blocker is created because of the manual update or deletion of a service instance. The summary describes the blocker as being active or resolved.</p>
layout: schema
name: ServiceSyncBlockerSummary
properties_list:
- description: ''
  name: latestBlockers
  type: object
- description: ''
  name: serviceInstanceName
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-service-sync-blocker-summary-schema.json
slug: amazon-proton-service-sync-blocker-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-sync-blocker-summary-schema.json\",\n  \"title\": \"ServiceSyncBlockerSummary\",\n  \"description\": \"<p>If a service instance is manually updated, Proton wants to prevent accidentally overriding a manual change.</p> <p>A blocker is created because of the manual update or deletion of a service instance. The summary describes the blocker as being active or resolved.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latestBlockers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LatestSyncBlockers\"\n        },\n        {\n          \"description\": \"The latest active blockers for the synced service.\"\n        }\n      ]\n    },\n    \"serviceInstanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The name of the service instance that you want sync your service configuration with.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The name of the service that you want to get the sync blocker summary for. If given a service instance name and a service name, it will return the blockers only applying to the instance that is blocked.</p> <p>If given only a service name, it will return the blockers that apply to all of the instances. In order to get the blockers for a single instance, you will need to make two distinct calls, one to get the sync blocker summary for the service and the other to get the sync blocker for the service instance.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-sync-blocker-summary-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ServiceSyncBlockerSummary
---
