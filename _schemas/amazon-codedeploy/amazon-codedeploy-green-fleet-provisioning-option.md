---
description: Information about the instances that belong to the replacement environment in a blue/green deployment.
layout: schema
name: GreenFleetProvisioningOption
properties_list:
- description: ''
  name: action
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-green-fleet-provisioning-option-schema.json
slug: amazon-codedeploy-green-fleet-provisioning-option
source_filename: amazon-codedeploy-green-fleet-provisioning-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-green-fleet-provisioning-option-schema.json\",\n  \"title\": \"GreenFleetProvisioningOption\",\n  \"description\": \"Information about the instances that belong to the replacement environment in a blue/green deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GreenFleetProvisioningAction\"\n        },\n        {\n          \"description\": \"<p>The method used to add instances to a replacement environment.</p> <ul> <li> <p> <code>DISCOVER_EXISTING</code>: Use instances that already exist or will be created manually.</p> </li> <li> <p> <code>COPY_AUTO_SCALING_GROUP</code>: Use settings from a specified Auto Scaling group to define and create instances in a new Auto Scaling group.</p>\
  \ </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-green-fleet-provisioning-option-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GreenFleetProvisioningOption
---
