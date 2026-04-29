---
description: Information about a deployment.
layout: schema
name: DeploymentInfo
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
  name: deploymentId
  type: object
- description: ''
  name: previousRevision
  type: object
- description: ''
  name: revision
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: errorInformation
  type: object
- description: ''
  name: createTime
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: completeTime
  type: object
- description: ''
  name: deploymentOverview
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: creator
  type: object
- description: ''
  name: ignoreApplicationStopFailures
  type: object
- description: ''
  name: autoRollbackConfiguration
  type: object
- description: ''
  name: updateOutdatedInstancesOnly
  type: object
- description: ''
  name: rollbackInfo
  type: object
- description: ''
  name: deploymentStyle
  type: object
- description: ''
  name: targetInstances
  type: object
- description: ''
  name: instanceTerminationWaitTimeStarted
  type: object
- description: ''
  name: blueGreenDeploymentConfiguration
  type: object
- description: ''
  name: loadBalancerInfo
  type: object
- description: ''
  name: additionalDeploymentStatusInfo
  type: object
- description: ''
  name: fileExistsBehavior
  type: object
- description: ''
  name: deploymentStatusMessages
  type: object
- description: ''
  name: computePlatform
  type: object
- description: ''
  name: externalId
  type: object
- description: ''
  name: relatedDeployments
  type: object
- description: ''
  name: overrideAlarmConfiguration
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-deployment-info-schema.json
slug: amazon-codedeploy-deployment-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-info-schema.json\",\n  \"title\": \"DeploymentInfo\",\n  \"description\": \"Information about a deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The application name.\"\n        }\n      ]\n    },\n    \"deploymentGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupName\"\n        },\n        {\n          \"description\": \" The deployment group name. \"\n        }\n      ]\n    },\n    \"deploymentConfigName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigName\"\n        },\n        {\n  \
  \        \"description\": \" The deployment configuration name. \"\n        }\n      ]\n    },\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"previousRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocation\"\n        },\n        {\n          \"description\": \"Information about the application revision that was deployed to the deployment group before the most recent successful deployment.\"\n        }\n      ]\n    },\n    \"revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocation\"\n        },\n        {\n          \"description\": \"Information about the location of stored application artifacts and the service from which to retrieve them.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n        },\n        {\n          \"description\": \"The current state of the deployment as a whole.\"\n        }\n      ]\n    },\n    \"errorInformation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorInformation\"\n        },\n        {\n          \"description\": \"Information about any error associated with this deployment.\"\n        }\n      ]\n    },\n    \"createTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp that indicates when the deployment was created.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>A timestamp that indicates when the deployment was deployed to the deployment group.</p> <p>In some cases,\
  \ the reported value of the start time might be later than the complete time. This is due to differences in the clock settings of backend servers that participate in the deployment process.</p>\"\n        }\n      ]\n    },\n    \"completeTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp that indicates when the deployment was complete.\"\n        }\n      ]\n    },\n    \"deploymentOverview\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentOverview\"\n        },\n        {\n          \"description\": \"A summary of the deployment status of the instances in the deployment.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A comment about the deployment.\"\n        }\n      ]\n    },\n    \"creator\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentCreator\"\n        },\n        {\n          \"description\": \"<p>The means by which the deployment was created:</p> <ul> <li> <p> <code>user</code>: A user created the deployment.</p> </li> <li> <p> <code>autoscaling</code>: Amazon EC2 Auto Scaling created the deployment.</p> </li> <li> <p> <code>codeDeployRollback</code>: A rollback process created the deployment.</p> </li> <li> <p> <code>CodeDeployAutoUpdate</code>: An auto-update process created the deployment when it detected outdated Amazon EC2 instances.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ignoreApplicationStopFailures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p> If true, then if an <code>ApplicationStop</code>, <code>BeforeBlockTraffic</code>, or <code>AfterBlockTraffic</code> deployment lifecycle event to an instance fails,\
  \ then the deployment continues to the next deployment lifecycle event. For example, if <code>ApplicationStop</code> fails, the deployment continues with DownloadBundle. If <code>BeforeBlockTraffic</code> fails, the deployment continues with <code>BlockTraffic</code>. If <code>AfterBlockTraffic</code> fails, the deployment continues with <code>ApplicationStop</code>. </p> <p> If false or not specified, then if a lifecycle event fails during a deployment to an instance, that deployment fails. If deployment to that instance is part of an overall deployment and the number of healthy hosts is not less than the minimum number of healthy hosts, then a deployment to the next instance is attempted. </p> <p> During a deployment, the CodeDeploy agent runs the scripts specified for <code>ApplicationStop</code>, <code>BeforeBlockTraffic</code>, and <code>AfterBlockTraffic</code> in the AppSpec file from the previous successful deployment. (All other scripts are run from the AppSpec file in the current\
  \ deployment.) If one of these scripts contains an error and does not run successfully, the deployment can fail. </p> <p> If the cause of the failure is a script from the last successful deployment that will never run successfully, create a new deployment and use <code>ignoreApplicationStopFailures</code> to specify that the <code>ApplicationStop</code>, <code>BeforeBlockTraffic</code>, and <code>AfterBlockTraffic</code> failures should be ignored. </p>\"\n        }\n      ]\n    },\n    \"autoRollbackConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoRollbackConfiguration\"\n        },\n        {\n          \"description\": \"Information about the automatic rollback configuration associated with the deployment.\"\n        }\n      ]\n    },\n    \"updateOutdatedInstancesOnly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether only\
  \ instances that are not running the latest application revision are to be deployed to.\"\n        }\n      ]\n    },\n    \"rollbackInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RollbackInfo\"\n        },\n        {\n          \"description\": \"Information about a deployment rollback.\"\n        }\n      ]\n    },\n    \"deploymentStyle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStyle\"\n        },\n        {\n          \"description\": \"Information about the type of deployment, either in-place or blue/green, you want to run and whether to route deployment traffic behind a load balancer.\"\n        }\n      ]\n    },\n    \"targetInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetInstances\"\n        },\n        {\n          \"description\": \"Information about the instances that belong to the replacement environment in a blue/green deployment.\"\n     \
  \   }\n      ]\n    },\n    \"instanceTerminationWaitTimeStarted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether the wait period set for the termination of instances in the original environment has started. Status is 'false' if the KEEP_ALIVE option is specified. Otherwise, 'true' as soon as the termination wait period starts.\"\n        }\n      ]\n    },\n    \"blueGreenDeploymentConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlueGreenDeploymentConfiguration\"\n        },\n        {\n          \"description\": \"Information about blue/green deployment options for this deployment.\"\n        }\n      ]\n    },\n    \"loadBalancerInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoadBalancerInfo\"\n        },\n        {\n          \"description\": \"Information about the load balancer used in the\
  \ deployment.\"\n        }\n      ]\n    },\n    \"additionalDeploymentStatusInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDeploymentStatusInfo\"\n        },\n        {\n          \"description\": \"Provides information about the results of a deployment, such as whether instances in the original environment in a blue/green deployment were not terminated.\"\n        }\n      ]\n    },\n    \"fileExistsBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileExistsBehavior\"\n        },\n        {\n          \"description\": \"<p>Information about how CodeDeploy handles files that already exist in a deployment target location but weren't part of the previous successful deployment.</p> <ul> <li> <p> <code>DISALLOW</code>: The deployment fails. This is also the default behavior if no option is specified.</p> </li> <li> <p> <code>OVERWRITE</code>: The version of the file from the application revision currently\
  \ being deployed replaces the version already on the instance.</p> </li> <li> <p> <code>RETAIN</code>: The version of the file already on the instance is kept and used as part of the new deployment.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"deploymentStatusMessages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatusMessageList\"\n        },\n        {\n          \"description\": \"Messages that contain information about the status of a deployment.\"\n        }\n      ]\n    },\n    \"computePlatform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputePlatform\"\n        },\n        {\n          \"description\": \"The destination platform type for the deployment (<code>Lambda</code>, <code>Server</code>, or <code>ECS</code>).\"\n        }\n      ]\n    },\n    \"externalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalId\"\n        },\n        {\n        \
  \  \"description\": \"The unique ID for an external resource (for example, a CloudFormation stack ID) that is linked to this deployment.\"\n        }\n      ]\n    },\n    \"relatedDeployments\": {\n      \"$ref\": \"#/components/schemas/RelatedDeployments\"\n    },\n    \"overrideAlarmConfiguration\": {\n      \"$ref\": \"#/components/schemas/AlarmConfiguration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-info-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeploymentInfo
---
