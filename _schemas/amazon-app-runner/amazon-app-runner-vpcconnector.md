---
description: <p>Describes an App Runner VPC connector resource. A VPC connector describes the Amazon Virtual Private Cloud (Amazon VPC) that an App Runner service is associated with, and the subnets and security group that are used.</p> <p>Multiple revisions of a connector might have the same <code>Name</code> and different <code>Revision</code> values.</p> <note> <p>At this time, App Runner supports only one revision per name.</p> </note>
layout: schema
name: VpcConnector
properties_list:
- description: ''
  name: VpcConnectorName
  type: object
- description: ''
  name: VpcConnectorArn
  type: object
- description: ''
  name: VpcConnectorRevision
  type: object
- description: ''
  name: Subnets
  type: object
- description: ''
  name: SecurityGroups
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: DeletedAt
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-vpcconnector-schema.json
slug: amazon-app-runner-vpcconnector
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VpcConnector\",\n  \"description\": \"<p>Describes an App Runner VPC connector resource. A VPC connector describes the Amazon Virtual Private Cloud (Amazon VPC) that an App Runner service is associated with, and the subnets and security group that are used.</p> <p>Multiple revisions of a connector might have the same <code>Name</code> and different <code>Revision</code> values.</p> <note> <p>At this time, App Runner supports only one revision per name.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcConnectorName\": {},\n    \"VpcConnectorArn\": {},\n    \"VpcConnectorRevision\": {},\n    \"Subnets\": {},\n    \"SecurityGroups\": {},\n    \"Status\": {},\n    \"CreatedAt\": {},\n    \"DeletedAt\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-vpcconnector-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: VpcConnector
---
