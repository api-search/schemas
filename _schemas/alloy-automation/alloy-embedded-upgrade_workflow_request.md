---
description: Request body for upgrading a workflow
layout: schema
name: UpgradeWorkflowRequest
properties_list:
- description: Identifier of the user
  name: userId
  type: string
- description: Target version to upgrade to
  name: version
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-upgrade_workflow_request-schema.json
slug: alloy-embedded-upgrade_workflow_request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-upgrade_workflow_request-schema.json\",\n  \"title\": \"UpgradeWorkflowRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for upgrading a workflow\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Target version to upgrade to\"\n    }\n  },\n  \"required\": [\n    \"userId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-upgrade_workflow_request-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: UpgradeWorkflowRequest
---
