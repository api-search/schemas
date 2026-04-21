---
description: Stage schema from Amazon API Gateway v2 API
layout: schema
name: Stage
properties_list:
- description: Name of the stage.
  name: StageName
  type: string
- description: Deployment identifier.
  name: DeploymentId
  type: string
- description: Description of the stage.
  name: Description
  type: string
- description: Whether updates auto-deploy to this stage.
  name: AutoDeploy
  type: boolean
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-stage-schema.json
slug: v2-stage
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Stage
---
