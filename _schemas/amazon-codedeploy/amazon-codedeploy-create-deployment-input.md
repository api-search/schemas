---
description: Represents the input of a <code>CreateDeployment</code> operation.
layout: schema
name: CreateDeploymentInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: deploymentGroupName
  type: object
- description: ''
  name: revision
  type: object
- description: ''
  name: deploymentConfigName
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: ignoreApplicationStopFailures
  type: object
- description: ''
  name: targetInstances
  type: object
- description: ''
  name: autoRollbackConfiguration
  type: object
- description: ''
  name: updateOutdatedInstancesOnly
  type: object
- description: ''
  name: fileExistsBehavior
  type: object
- description: ''
  name: overrideAlarmConfiguration
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-create-deployment-input-schema.json
slug: amazon-codedeploy-create-deployment-input
source_filename: amazon-codedeploy-create-deployment-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-input-schema.json\",\n  \"title\": \"CreateDeploymentInput\",\n  \"description\": \"Represents the input of a <code>CreateDeployment</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of an CodeDeploy application associated with the IAM user or Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"deploymentGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupName\"\n        },\n        {\n          \"description\": \"The name of the deployment group.\"\n        }\n      ]\n    },\n    \"revision\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocation\"\n        },\n        {\n          \"description\": \" The type and location of the revision to deploy. \"\n        }\n      ]\n    },\n    \"deploymentConfigName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigName\"\n        },\n        {\n          \"description\": \"<p>The name of a deployment configuration associated with the IAM user or Amazon Web Services account.</p> <p>If not specified, the value configured in the deployment group is used as the default. If the deployment group does not have a deployment configuration associated with it, <code>CodeDeployDefault</code>.<code>OneAtATime</code> is used by default.</p>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A comment about the deployment.\"\n\
  \        }\n      ]\n    },\n    \"ignoreApplicationStopFailures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p> If true, then if an <code>ApplicationStop</code>, <code>BeforeBlockTraffic</code>, or <code>AfterBlockTraffic</code> deployment lifecycle event to an instance fails, then the deployment continues to the next deployment lifecycle event. For example, if <code>ApplicationStop</code> fails, the deployment continues with <code>DownloadBundle</code>. If <code>BeforeBlockTraffic</code> fails, the deployment continues with <code>BlockTraffic</code>. If <code>AfterBlockTraffic</code> fails, the deployment continues with <code>ApplicationStop</code>. </p> <p> If false or not specified, then if a lifecycle event fails during a deployment to an instance, that deployment fails. If deployment to that instance is part of an overall deployment and the number of healthy hosts is not less than the\
  \ minimum number of healthy hosts, then a deployment to the next instance is attempted. </p> <p> During a deployment, the CodeDeploy agent runs the scripts specified for <code>ApplicationStop</code>, <code>BeforeBlockTraffic</code>, and <code>AfterBlockTraffic</code> in the AppSpec file from the previous successful deployment. (All other scripts are run from the AppSpec file in the current deployment.) If one of these scripts contains an error and does not run successfully, the deployment can fail. </p> <p> If the cause of the failure is a script from the last successful deployment that will never run successfully, create a new deployment and use <code>ignoreApplicationStopFailures</code> to specify that the <code>ApplicationStop</code>, <code>BeforeBlockTraffic</code>, and <code>AfterBlockTraffic</code> failures should be ignored. </p>\"\n        }\n      ]\n    },\n    \"targetInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetInstances\"\n\
  \        },\n        {\n          \"description\": \" Information about the instances that belong to the replacement environment in a blue/green deployment. \"\n        }\n      ]\n    },\n    \"autoRollbackConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoRollbackConfiguration\"\n        },\n        {\n          \"description\": \"Configuration information for an automatic rollback that is added when a deployment is created.\"\n        }\n      ]\n    },\n    \"updateOutdatedInstancesOnly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Indicates whether to deploy to all instances or only to instances that are not running the latest application revision. \"\n        }\n      ]\n    },\n    \"fileExistsBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileExistsBehavior\"\n        },\n        {\n          \"\
  description\": \"<p>Information about how CodeDeploy handles files that already exist in a deployment target location but weren't part of the previous successful deployment.</p> <p>The <code>fileExistsBehavior</code> parameter takes any of the following values:</p> <ul> <li> <p>DISALLOW: The deployment fails. This is also the default behavior if no option is specified.</p> </li> <li> <p>OVERWRITE: The version of the file from the application revision currently being deployed replaces the version already on the instance.</p> </li> <li> <p>RETAIN: The version of the file already on the instance is kept and used as part of the new deployment.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"overrideAlarmConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmConfiguration\"\n        },\n        {\n          \"description\": \"<p>Allows you to specify information about alarms associated with a deployment. The alarm configuration that you specify\
  \ here will override the alarm configuration at the deployment group level. Consider overriding the alarm configuration if you have set up alarms at the deployment group level that are causing deployment failures. In this case, you would call <code>CreateDeployment</code> to create a new deployment that uses a previous application revision that is known to work, and set its alarm configuration to turn off alarm polling. Turning off alarm polling ensures that the new deployment proceeds without being blocked by the alarm that was generated by the previous, failed, deployment.</p> <note> <p>If you specify an <code>overrideAlarmConfiguration</code>, you need the <code>UpdateDeploymentGroup</code> IAM permission when calling <code>CreateDeployment</code>.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: CreateDeploymentInput
---
