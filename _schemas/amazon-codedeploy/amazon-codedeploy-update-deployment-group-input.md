---
description: Represents the input of an <code>UpdateDeploymentGroup</code> operation.
layout: schema
name: UpdateDeploymentGroupInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: currentDeploymentGroupName
  type: object
- description: ''
  name: newDeploymentGroupName
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
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-update-deployment-group-input-schema.json
slug: amazon-codedeploy-update-deployment-group-input
source_filename: amazon-codedeploy-update-deployment-group-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-update-deployment-group-input-schema.json\",\n  \"title\": \"UpdateDeploymentGroupInput\",\n  \"description\": \"Represents the input of an <code>UpdateDeploymentGroup</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The application name that corresponds to the deployment group to update.\"\n        }\n      ]\n    },\n    \"currentDeploymentGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupName\"\n        },\n        {\n          \"description\": \"The current name of the deployment group.\"\n        }\n      ]\n    },\n    \"newDeploymentGroupName\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupName\"\n        },\n        {\n          \"description\": \"The new name of the deployment group, if you want to change it.\"\n        }\n      ]\n    },\n    \"deploymentConfigName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigName\"\n        },\n        {\n          \"description\": \"The replacement deployment configuration name to use, if you want to change it.\"\n        }\n      ]\n    },\n    \"ec2TagFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2TagFilterList\"\n        },\n        {\n          \"description\": \"The replacement set of Amazon EC2 tags on which to filter, if you want to change them. To keep the existing tags, enter their names. To remove tags, do not enter any tag names.\"\n        }\n      ]\n    },\n    \"onPremisesInstanceTagFilters\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/TagFilterList\"\n        },\n        {\n          \"description\": \"The replacement set of on-premises instance tags on which to filter, if you want to change them. To keep the existing tags, enter their names. To remove tags, do not enter any tag names.\"\n        }\n      ]\n    },\n    \"autoScalingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupNameList\"\n        },\n        {\n          \"description\": \"<p>The replacement list of Auto Scaling groups to be included in the deployment group, if you want to change them.</p> <ul> <li> <p>To keep the Auto Scaling groups, enter their names or do not specify this parameter. </p> </li> <li> <p>To remove Auto Scaling groups, specify a non-null empty list of Auto Scaling group names to detach all CodeDeploy-managed Auto Scaling lifecycle hooks. For examples, see <a href=\\\"https://docs.aws.amazon.com/https:/docs.aws.amazon.com/codedeploy/latest/userguide/troubleshooting-auto-scaling.html#troubleshooting-auto-scaling-heartbeat\\\
  \">Amazon EC2 instances in an Amazon EC2 Auto Scaling group fail to launch and receive the error \\\"Heartbeat Timeout\\\"</a> in the <i>CodeDeploy User Guide</i>.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"serviceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"A replacement ARN for the service role, if you want to change it.\"\n        }\n      ]\n    },\n    \"triggerConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerConfigList\"\n        },\n        {\n          \"description\": \"Information about triggers to change when the deployment group is updated. For examples, see <a href=\\\"https://docs.aws.amazon.com/codedeploy/latest/userguide/how-to-notify-edit.html\\\">Edit a Trigger in a CodeDeploy Deployment Group</a> in the <i>CodeDeploy User Guide</i>.\"\n        }\n      ]\n    },\n    \"alarmConfiguration\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/AlarmConfiguration\"\n        },\n        {\n          \"description\": \"Information to add or change about Amazon CloudWatch alarms when the deployment group is updated.\"\n        }\n      ]\n    },\n    \"autoRollbackConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoRollbackConfiguration\"\n        },\n        {\n          \"description\": \"Information for an automatic rollback configuration that is added or changed when a deployment group is updated.\"\n        }\n      ]\n    },\n    \"outdatedInstancesStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutdatedInstancesStrategy\"\n        },\n        {\n          \"description\": \"<p>Indicates what happens when new Amazon EC2 instances are launched mid-deployment and do not receive the deployed application revision.</p> <p>If this option is set to <code>UPDATE</code> or is unspecified,\
  \ CodeDeploy initiates one or more 'auto-update outdated instances' deployments to apply the deployed application revision to the new Amazon EC2 instances.</p> <p>If this option is set to <code>IGNORE</code>, CodeDeploy does not initiate a deployment to update the new Amazon EC2 instances. This may result in instances having different revisions.</p>\"\n        }\n      ]\n    },\n    \"deploymentStyle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStyle\"\n        },\n        {\n          \"description\": \"Information about the type of deployment, either in-place or blue/green, you want to run and whether to route deployment traffic behind a load balancer.\"\n        }\n      ]\n    },\n    \"blueGreenDeploymentConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlueGreenDeploymentConfiguration\"\n        },\n        {\n          \"description\": \"Information about blue/green deployment options for a\
  \ deployment group.\"\n        }\n      ]\n    },\n    \"loadBalancerInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoadBalancerInfo\"\n        },\n        {\n          \"description\": \"Information about the load balancer used in a deployment.\"\n        }\n      ]\n    },\n    \"ec2TagSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2TagSet\"\n        },\n        {\n          \"description\": \"Information about groups of tags applied to on-premises instances. The deployment group includes only Amazon EC2 instances identified by all the tag groups.\"\n        }\n      ]\n    },\n    \"ecsServices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceList\"\n        },\n        {\n          \"description\": \" The target Amazon ECS services in the deployment group. This applies only to deployment groups that use the Amazon ECS compute platform. A target Amazon ECS service is\
  \ specified as an Amazon ECS cluster and service name pair using the format <code>&lt;clustername&gt;:&lt;servicename&gt;</code>. \"\n        }\n      ]\n    },\n    \"onPremisesTagSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnPremisesTagSet\"\n        },\n        {\n          \"description\": \"Information about an on-premises instance tag set. The deployment group includes only on-premises instances identified by all the tag groups.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationName\",\n    \"currentDeploymentGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-update-deployment-group-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: UpdateDeploymentGroupInput
---
