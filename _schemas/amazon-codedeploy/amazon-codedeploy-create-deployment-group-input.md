---
description: Represents the input of a <code>CreateDeploymentGroup</code> operation.
layout: schema
name: CreateDeploymentGroupInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: deploymentGroupName
  type: object
- description: ''
  name: deploymentConfigName
  type: object
- description: ''
  name: ec2TagFilters
  type: object
- description: ''
  name: onPremisesInstanceTagFilters
  type: object
- description: ''
  name: autoScalingGroups
  type: object
- description: ''
  name: serviceRoleArn
  type: object
- description: ''
  name: triggerConfigurations
  type: object
- description: ''
  name: alarmConfiguration
  type: object
- description: ''
  name: autoRollbackConfiguration
  type: object
- description: ''
  name: outdatedInstancesStrategy
  type: object
- description: ''
  name: deploymentStyle
  type: object
- description: ''
  name: blueGreenDeploymentConfiguration
  type: object
- description: ''
  name: loadBalancerInfo
  type: object
- description: ''
  name: ec2TagSet
  type: object
- description: ''
  name: ecsServices
  type: object
- description: ''
  name: onPremisesTagSet
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-create-deployment-group-input-schema.json
slug: amazon-codedeploy-create-deployment-group-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-group-input-schema.json\",\n  \"title\": \"CreateDeploymentGroupInput\",\n  \"description\": \"Represents the input of a <code>CreateDeploymentGroup</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of an CodeDeploy application associated with the IAM user or Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"deploymentGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupName\"\n        },\n        {\n          \"description\": \"The name of a new deployment group for the specified application.\"\n    \
  \    }\n      ]\n    },\n    \"deploymentConfigName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigName\"\n        },\n        {\n          \"description\": \"<p>If specified, the deployment configuration name can be either one of the predefined configurations provided with CodeDeploy or a custom deployment configuration that you create by calling the create deployment configuration operation.</p> <p> <code>CodeDeployDefault.OneAtATime</code> is the default deployment configuration. It is used if a configuration isn't specified for the deployment or deployment group.</p> <p>For more information about the predefined deployment configurations in CodeDeploy, see <a href=\\\"https://docs.aws.amazon.com/codedeploy/latest/userguide/deployment-configurations.html\\\">Working with Deployment Configurations in CodeDeploy</a> in the <i>CodeDeploy User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"ec2TagFilters\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/EC2TagFilterList\"\n        },\n        {\n          \"description\": \"The Amazon EC2 tags on which to filter. The deployment group includes Amazon EC2 instances with any of the specified tags. Cannot be used in the same call as ec2TagSet.\"\n        }\n      ]\n    },\n    \"onPremisesInstanceTagFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagFilterList\"\n        },\n        {\n          \"description\": \"The on-premises instance tags on which to filter. The deployment group includes on-premises instances with any of the specified tags. Cannot be used in the same call as <code>OnPremisesTagSet</code>.\"\n        }\n      ]\n    },\n    \"autoScalingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupNameList\"\n        },\n        {\n          \"description\": \"A list of associated Amazon EC2 Auto Scaling groups.\"\n        }\n      ]\n \
  \   },\n    \"serviceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"A service role Amazon Resource Name (ARN) that allows CodeDeploy to act on the user's behalf when interacting with Amazon Web Services services.\"\n        }\n      ]\n    },\n    \"triggerConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerConfigList\"\n        },\n        {\n          \"description\": \"Information about triggers to create when the deployment group is created. For examples, see <a href=\\\"https://docs.aws.amazon.com/codedeploy/latest/userguide/how-to-notify-sns.html\\\">Create a Trigger for an CodeDeploy Event</a> in the <i>CodeDeploy User Guide</i>.\"\n        }\n      ]\n    },\n    \"alarmConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmConfiguration\"\n        },\n        {\n          \"description\"\
  : \"Information to add about Amazon CloudWatch alarms when the deployment group is created.\"\n        }\n      ]\n    },\n    \"autoRollbackConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoRollbackConfiguration\"\n        },\n        {\n          \"description\": \"Configuration information for an automatic rollback that is added when a deployment group is created.\"\n        }\n      ]\n    },\n    \"outdatedInstancesStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutdatedInstancesStrategy\"\n        },\n        {\n          \"description\": \"<p>Indicates what happens when new Amazon EC2 instances are launched mid-deployment and do not receive the deployed application revision.</p> <p>If this option is set to <code>UPDATE</code> or is unspecified, CodeDeploy initiates one or more 'auto-update outdated instances' deployments to apply the deployed application revision to the new Amazon EC2 instances.</p>\
  \ <p>If this option is set to <code>IGNORE</code>, CodeDeploy does not initiate a deployment to update the new Amazon EC2 instances. This may result in instances having different revisions.</p>\"\n        }\n      ]\n    },\n    \"deploymentStyle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStyle\"\n        },\n        {\n          \"description\": \"Information about the type of deployment, in-place or blue/green, that you want to run and whether to route deployment traffic behind a load balancer.\"\n        }\n      ]\n    },\n    \"blueGreenDeploymentConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlueGreenDeploymentConfiguration\"\n        },\n        {\n          \"description\": \"Information about blue/green deployment options for a deployment group.\"\n        }\n      ]\n    },\n    \"loadBalancerInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoadBalancerInfo\"\
  \n        },\n        {\n          \"description\": \"Information about the load balancer used in a deployment.\"\n        }\n      ]\n    },\n    \"ec2TagSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2TagSet\"\n        },\n        {\n          \"description\": \"Information about groups of tags applied to Amazon EC2 instances. The deployment group includes only Amazon EC2 instances identified by all the tag groups. Cannot be used in the same call as <code>ec2TagFilters</code>.\"\n        }\n      ]\n    },\n    \"ecsServices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceList\"\n        },\n        {\n          \"description\": \" The target Amazon ECS services in the deployment group. This applies only to deployment groups that use the Amazon ECS compute platform. A target Amazon ECS service is specified as an Amazon ECS cluster and service name pair using the format <code>&lt;clustername&gt;:&lt;servicename&gt;</code>.\
  \ \"\n        }\n      ]\n    },\n    \"onPremisesTagSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnPremisesTagSet\"\n        },\n        {\n          \"description\": \"Information about groups of tags applied to on-premises instances. The deployment group includes only on-premises instances identified by all of the tag groups. Cannot be used in the same call as <code>onPremisesInstanceTagFilters</code>.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \" The metadata that you apply to CodeDeploy deployment groups to help you organize and categorize them. Each tag consists of a key and an optional value, both of which you define. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationName\",\n    \"deploymentGroupName\",\n    \"serviceRoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-group-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: CreateDeploymentGroupInput
---
