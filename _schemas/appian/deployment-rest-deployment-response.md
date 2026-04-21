---
description: Response returned when a deployment operation is successfully initiated. Contains the UUID for tracking the deployment and its current status.
layout: schema
name: DeploymentResponse
properties_list:
- description: Unique identifier for the deployment operation. Use this UUID to retrieve deployment results and logs.
  name: uuid
  type: string
- description: URL endpoint for retrieving the deployment details and results.
  name: url
  type: string
- description: ''
  name: status
  type: object
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-deployment-response-schema.json
slug: deployment-rest-deployment-response
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: DeploymentResponse
---
