---
description: The current status of a deployment operation. IN_PROGRESS indicates the operation is still running. COMPLETED indicates success. Other statuses indicate various error or review states.
layout: schema
name: DeploymentStatus
properties_list: []
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-deployment-status-schema.json
slug: deployment-rest-deployment-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-deployment-status-schema.json\",\n  \"title\": \"DeploymentStatus\",\n  \"description\": \"The current status of a deployment operation. IN_PROGRESS indicates the operation is still running. COMPLETED indicates success. Other statuses indicate various error or review states.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"IN_PROGRESS\",\n    \"COMPLETED\",\n    \"COMPLETED_WITH_ERRORS\",\n    \"COMPLETED_WITH_IMPORT_ERRORS\",\n    \"COMPLETED_WITH_PUBLISH_ERRORS\",\n    \"FAILED\",\n    \"PENDING_REVIEW\",\n    \"REJECTED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-deployment-status-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: DeploymentStatus
---
