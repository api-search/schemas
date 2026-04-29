---
description: Information about how traffic is rerouted to instances in a replacement environment in a blue/green deployment.
layout: schema
name: DeploymentReadyOption
properties_list:
- description: ''
  name: actionOnTimeout
  type: object
- description: ''
  name: waitTimeInMinutes
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-deployment-ready-option-schema.json
slug: amazon-codedeploy-deployment-ready-option
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-ready-option-schema.json\",\n  \"title\": \"DeploymentReadyOption\",\n  \"description\": \"Information about how traffic is rerouted to instances in a replacement environment in a blue/green deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionOnTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentReadyAction\"\n        },\n        {\n          \"description\": \"<p>Information about when to reroute traffic from an original environment to a replacement environment in a blue/green deployment.</p> <ul> <li> <p>CONTINUE_DEPLOYMENT: Register new instances with the load balancer immediately after the new application revision is installed on the instances in the replacement environment.</p> </li> <li> <p>STOP_DEPLOYMENT:\
  \ Do not register new instances with a load balancer unless traffic rerouting is started using <a>ContinueDeployment</a>. If traffic rerouting is not started before the end of the specified wait period, the deployment status is changed to Stopped.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"waitTimeInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"The number of minutes to wait before the status of a blue/green deployment is changed to Stopped if rerouting is not started manually. Applies only to the <code>STOP_DEPLOYMENT</code> option for <code>actionOnTimeout</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-ready-option-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeploymentReadyOption
---
