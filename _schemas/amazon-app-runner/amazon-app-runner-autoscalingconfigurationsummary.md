---
description: <p>Provides summary information about an App Runner automatic scaling configuration resource.</p> <p>This type contains limited information about an auto scaling configuration. It includes only identification information, without configuration details. It's returned by the <a>ListAutoScalingConfigurations</a> action. Complete configuration information is returned by the <a>CreateAutoScalingConfiguration</a>, <a>DescribeAutoScalingConfiguration</a>, and <a>DeleteAutoScalingConfiguration</a> actions using the <a>AutoScalingConfiguration</a> type.</p>
layout: schema
name: AutoScalingConfigurationSummary
properties_list:
- description: ''
  name: AutoScalingConfigurationArn
  type: object
- description: ''
  name: AutoScalingConfigurationName
  type: object
- description: ''
  name: AutoScalingConfigurationRevision
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-autoscalingconfigurationsummary-schema.json
slug: amazon-app-runner-autoscalingconfigurationsummary
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AutoScalingConfigurationSummary\",\n  \"description\": \"<p>Provides summary information about an App Runner automatic scaling configuration resource.</p> <p>This type contains limited information about an auto scaling configuration. It includes only identification information, without configuration details. It's returned by the <a>ListAutoScalingConfigurations</a> action. Complete configuration information is returned by the <a>CreateAutoScalingConfiguration</a>, <a>DescribeAutoScalingConfiguration</a>, and <a>DeleteAutoScalingConfiguration</a> actions using the <a>AutoScalingConfiguration</a> type.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingConfigurationArn\": {},\n    \"AutoScalingConfigurationName\": {},\n    \"AutoScalingConfigurationRevision\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-autoscalingconfigurationsummary-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: AutoScalingConfigurationSummary
---
