---
description: Information about minimum healthy instance.
layout: schema
name: MinimumHealthyHosts
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-minimum-healthy-hosts-schema.json
slug: amazon-codedeploy-minimum-healthy-hosts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-minimum-healthy-hosts-schema.json\",\n  \"title\": \"MinimumHealthyHosts\",\n  \"description\": \"Information about minimum healthy instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinimumHealthyHostsType\"\n        },\n        {\n          \"description\": \"<p>The minimum healthy instance type:</p> <ul> <li> <p> <code>HOST_COUNT</code>: The minimum number of healthy instances as an absolute value.</p> </li> <li> <p> <code>FLEET_PERCENT</code>: The minimum number of healthy instances as a percentage of the total number of instances in the deployment.</p> </li> </ul> <p>In an example of nine instances, if a HOST_COUNT of six is specified, deploy to up to three instances at a time. The\
  \ deployment is successful if six or more instances are deployed to successfully. Otherwise, the deployment fails. If a FLEET_PERCENT of 40 is specified, deploy to up to five instances at a time. The deployment is successful if four or more instances are deployed to successfully. Otherwise, the deployment fails.</p> <note> <p>In a call to the <code>GetDeploymentConfig</code>, CodeDeployDefault.OneAtATime returns a minimum healthy instance type of MOST_CONCURRENCY and a value of 1. This means a deployment to only one instance at a time. (You cannot set the type to MOST_CONCURRENCY, only to HOST_COUNT or FLEET_PERCENT.) In addition, with CodeDeployDefault.OneAtATime, CodeDeploy attempts to ensure that all instances but one are kept in a healthy state during the deployment. Although this allows one instance at a time to be taken offline for a new deployment, it also means that if the deployment to the last instance fails, the overall deployment is still successful.</p> </note> <p>For more\
  \ information, see <a href=\\\"https://docs.aws.amazon.com/codedeploy/latest/userguide/instances-health.html\\\">CodeDeploy Instance Health</a> in the <i>CodeDeploy User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinimumHealthyHostsValue\"\n        },\n        {\n          \"description\": \"The minimum healthy instance value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-minimum-healthy-hosts-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: MinimumHealthyHosts
---
