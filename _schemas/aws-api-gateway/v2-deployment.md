---
description: Deployment schema from Amazon API Gateway v2 API
layout: schema
name: Deployment
properties_list:
- description: Deployment identifier.
  name: DeploymentId
  type: string
- description: Description of the deployment.
  name: Description
  type: string
- description: Status of the deployment (PENDING, FAILED, DEPLOYED).
  name: DeploymentStatus
  type: string
- description: Timestamp when the deployment was created.
  name: CreatedDate
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-deployment-schema.json
slug: v2-deployment
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Deployment
---
