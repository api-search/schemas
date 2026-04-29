---
description: Information about a deployment group.
layout: schema
name: DeploymentGroupInfo
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: deploymentGroupId
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
  name: targetRevision
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
  name: deploymentStyle
  type: object
- description: ''
  name: outdatedInstancesStrategy
  type: object
- description: ''
  name: blueGreenDeploymentConfiguration
  type: object
- description: ''
  name: loadBalancerInfo
  type: object
- description: ''
  name: lastSuccessfulDeployment
  type: object
- description: ''
  name: lastAttemptedDeployment
  type: object
- description: ''
  name: ec2TagSet
  type: object
- description: ''
  name: onPremisesTagSet
  type: object
- description: ''
  name: computePlatform
  type: object
- description: ''
  name: ecsServices
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-deployment-group-info-schema.json
slug: amazon-codedeploy-deployment-group-info
source_filename: amazon-codedeploy-deployment-group-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-group-info-schema.json\",\n  \"title\": \"DeploymentGroupInfo\",\n  \"description\": \"Information about a deployment group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The application name.\"\n        }\n      ]\n    },\n    \"deploymentGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupId\"\n        },\n        {\n          \"description\": \"The deployment group ID.\"\n        }\n      ]\n    },\n    \"deploymentGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupName\"\n        },\n      \
  \  {\n          \"description\": \"The deployment group name.\"\n        }\n      ]\n    },\n    \"deploymentConfigName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigName\"\n        },\n        {\n          \"description\": \"The deployment configuration name.\"\n        }\n      ]\n    },\n    \"ec2TagFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2TagFilterList\"\n        },\n        {\n          \"description\": \"The Amazon EC2 tags on which to filter. The deployment group includes EC2 instances with any of the specified tags.\"\n        }\n      ]\n    },\n    \"onPremisesInstanceTagFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagFilterList\"\n        },\n        {\n          \"description\": \"The on-premises instance tags on which to filter. The deployment group includes on-premises instances with any of the specified tags.\"\n        }\n      ]\n\
  \    },\n    \"autoScalingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupList\"\n        },\n        {\n          \"description\": \"A list of associated Auto Scaling groups.\"\n        }\n      ]\n    },\n    \"serviceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"A service role Amazon Resource Name (ARN) that grants CodeDeploy permission to make calls to Amazon Web Services services on your behalf. For more information, see <a href=\\\"https://docs.aws.amazon.com/codedeploy/latest/userguide/getting-started-create-service-role.html\\\">Create a Service Role for CodeDeploy</a> in the <i>CodeDeploy User Guide</i>.\"\n        }\n      ]\n    },\n    \"targetRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocation\"\n        },\n        {\n          \"description\": \"Information about\
  \ the deployment group's target revision, including type and location.\"\n        }\n      ]\n    },\n    \"triggerConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerConfigList\"\n        },\n        {\n          \"description\": \"Information about triggers associated with the deployment group.\"\n        }\n      ]\n    },\n    \"alarmConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmConfiguration\"\n        },\n        {\n          \"description\": \"A list of alarms associated with the deployment group.\"\n        }\n      ]\n    },\n    \"autoRollbackConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoRollbackConfiguration\"\n        },\n        {\n          \"description\": \"Information about the automatic rollback configuration associated with the deployment group.\"\n        }\n      ]\n    },\n    \"deploymentStyle\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStyle\"\n        },\n        {\n          \"description\": \"Information about the type of deployment, either in-place or blue/green, you want to run and whether to route deployment traffic behind a load balancer.\"\n        }\n      ]\n    },\n    \"outdatedInstancesStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutdatedInstancesStrategy\"\n        },\n        {\n          \"description\": \"<p>Indicates what happens when new Amazon EC2 instances are launched mid-deployment and do not receive the deployed application revision.</p> <p>If this option is set to <code>UPDATE</code> or is unspecified, CodeDeploy initiates one or more 'auto-update outdated instances' deployments to apply the deployed application revision to the new Amazon EC2 instances.</p> <p>If this option is set to <code>IGNORE</code>, CodeDeploy does not initiate a deployment to update the new Amazon EC2 instances.\
  \ This may result in instances having different revisions.</p>\"\n        }\n      ]\n    },\n    \"blueGreenDeploymentConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlueGreenDeploymentConfiguration\"\n        },\n        {\n          \"description\": \"Information about blue/green deployment options for a deployment group.\"\n        }\n      ]\n    },\n    \"loadBalancerInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoadBalancerInfo\"\n        },\n        {\n          \"description\": \"Information about the load balancer to use in a deployment.\"\n        }\n      ]\n    },\n    \"lastSuccessfulDeployment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastDeploymentInfo\"\n        },\n        {\n          \"description\": \"Information about the most recent successful deployment to the deployment group.\"\n        }\n      ]\n    },\n    \"lastAttemptedDeployment\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastDeploymentInfo\"\n        },\n        {\n          \"description\": \"Information about the most recent attempted deployment to the deployment group.\"\n        }\n      ]\n    },\n    \"ec2TagSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2TagSet\"\n        },\n        {\n          \"description\": \"Information about groups of tags applied to an Amazon EC2 instance. The deployment group includes only Amazon EC2 instances identified by all of the tag groups. Cannot be used in the same call as ec2TagFilters.\"\n        }\n      ]\n    },\n    \"onPremisesTagSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnPremisesTagSet\"\n        },\n        {\n          \"description\": \"Information about groups of tags applied to an on-premises instance. The deployment group includes only on-premises instances identified by all the tag groups.\
  \ Cannot be used in the same call as onPremisesInstanceTagFilters.\"\n        }\n      ]\n    },\n    \"computePlatform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputePlatform\"\n        },\n        {\n          \"description\": \"The destination platform type for the deployment (<code>Lambda</code>, <code>Server</code>, or <code>ECS</code>).\"\n        }\n      ]\n    },\n    \"ecsServices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceList\"\n        },\n        {\n          \"description\": \" The target Amazon ECS services in the deployment group. This applies only to deployment groups that use the Amazon ECS compute platform. A target Amazon ECS service is specified as an Amazon ECS cluster and service name pair using the format <code>&lt;clustername&gt;:&lt;servicename&gt;</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-group-info-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeploymentGroupInfo
---
