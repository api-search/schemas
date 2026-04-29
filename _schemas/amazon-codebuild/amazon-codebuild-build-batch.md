---
description: Contains information about a batch build.
layout: schema
name: BuildBatch
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: currentPhase
  type: object
- description: ''
  name: buildBatchStatus
  type: object
- description: ''
  name: sourceVersion
  type: object
- description: ''
  name: resolvedSourceVersion
  type: object
- description: ''
  name: projectName
  type: object
- description: ''
  name: phases
  type: object
- description: ''
  name: source
  type: object
- description: ''
  name: secondarySources
  type: object
- description: ''
  name: secondarySourceVersions
  type: object
- description: ''
  name: artifacts
  type: object
- description: ''
  name: secondaryArtifacts
  type: object
- description: ''
  name: cache
  type: object
- description: ''
  name: environment
  type: object
- description: ''
  name: serviceRole
  type: object
- description: ''
  name: logConfig
  type: object
- description: ''
  name: buildTimeoutInMinutes
  type: object
- description: ''
  name: queuedTimeoutInMinutes
  type: object
- description: ''
  name: complete
  type: object
- description: ''
  name: initiator
  type: object
- description: ''
  name: vpcConfig
  type: object
- description: ''
  name: encryptionKey
  type: object
- description: ''
  name: buildBatchNumber
  type: object
- description: ''
  name: fileSystemLocations
  type: object
- description: ''
  name: buildBatchConfig
  type: object
- description: ''
  name: buildGroups
  type: object
- description: ''
  name: debugSessionEnabled
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-build-batch-schema.json
slug: amazon-codebuild-build-batch
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-batch-schema.json\",\n  \"title\": \"BuildBatch\",\n  \"description\": \"Contains information about a batch build.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The identifier of the batch build.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ARN of the batch build.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that\
  \ the batch build started.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the batch build ended.\"\n        }\n      ]\n    },\n    \"currentPhase\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The current phase of the batch build.\"\n        }\n      ]\n    },\n    \"buildBatchStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusType\"\n        },\n        {\n          \"description\": \"The status of the batch build.\"\n        }\n      ]\n    },\n    \"sourceVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The identifier of the version of the source code to be built.\"\n        }\n\
  \      ]\n    },\n    \"resolvedSourceVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The identifier of the resolved version of this batch build's source code.</p> <ul> <li> <p>For CodeCommit, GitHub, GitHub Enterprise, and BitBucket, the commit ID.</p> </li> <li> <p>For CodePipeline, the source revision provided by CodePipeline.</p> </li> <li> <p>For Amazon S3, this does not apply.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the batch build project.\"\n        }\n      ]\n    },\n    \"phases\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildBatchPhases\"\n        },\n        {\n          \"description\": \"An array of <code>BuildBatchPhase</code> objects the\
  \ specify the phases of the batch build.\"\n        }\n      ]\n    },\n    \"source\": {\n      \"$ref\": \"#/components/schemas/ProjectSource\"\n    },\n    \"secondarySources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectSources\"\n        },\n        {\n          \"description\": \"An array of <code>ProjectSource</code> objects that define the sources for the batch build.\"\n        }\n      ]\n    },\n    \"secondarySourceVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectSecondarySourceVersions\"\n        },\n        {\n          \"description\": \"<p>An array of <code>ProjectSourceVersion</code> objects. Each <code>ProjectSourceVersion</code> must be one of: </p> <ul> <li> <p>For CodeCommit: the commit ID, branch, or Git tag to use.</p> </li> <li> <p>For GitHub: the commit ID, pull request ID, branch name, or tag name that corresponds to the version of the source code you want to build. If a pull\
  \ request ID is specified, it must use the format <code>pr/pull-request-ID</code> (for example, <code>pr/25</code>). If a branch name is specified, the branch's HEAD commit ID is used. If not specified, the default branch's HEAD commit ID is used.</p> </li> <li> <p>For Bitbucket: the commit ID, branch name, or tag name that corresponds to the version of the source code you want to build. If a branch name is specified, the branch's HEAD commit ID is used. If not specified, the default branch's HEAD commit ID is used.</p> </li> <li> <p>For Amazon S3: the version ID of the object that represents the build input ZIP file to use.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"artifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildArtifacts\"\n        },\n        {\n          \"description\": \"A <code>BuildArtifacts</code> object the defines the build artifacts for this batch build.\"\n        }\n      ]\n    },\n    \"secondaryArtifacts\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildArtifactsList\"\n        },\n        {\n          \"description\": \"An array of <code>BuildArtifacts</code> objects the define the build artifacts for this batch build.\"\n        }\n      ]\n    },\n    \"cache\": {\n      \"$ref\": \"#/components/schemas/ProjectCache\"\n    },\n    \"environment\": {\n      \"$ref\": \"#/components/schemas/ProjectEnvironment\"\n    },\n    \"serviceRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of a service role used for builds in the batch.\"\n        }\n      ]\n    },\n    \"logConfig\": {\n      \"$ref\": \"#/components/schemas/LogsConfig\"\n    },\n    \"buildTimeoutInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperInt\"\n        },\n        {\n          \"description\": \"Specifies the maximum amount of\
  \ time, in minutes, that the build in a batch must be completed in.\"\n        }\n      ]\n    },\n    \"queuedTimeoutInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperInt\"\n        },\n        {\n          \"description\": \"Specifies the amount of time, in minutes, that the batch build is allowed to be queued before it times out.\"\n        }\n      ]\n    },\n    \"complete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates if the batch build is complete.\"\n        }\n      ]\n    },\n    \"initiator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The entity that started the batch build. Valid values include:</p> <ul> <li> <p>If CodePipeline started the build, the pipeline's name (for example, <code>codepipeline/my-demo-pipeline</code>).</p>\
  \ </li> <li> <p>If an IAM user started the build, the user's name.</p> </li> <li> <p>If the Jenkins plugin for CodeBuild started the build, the string <code>CodeBuild-Jenkins-Plugin</code>.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"vpcConfig\": {\n      \"$ref\": \"#/components/schemas/VpcConfig\"\n    },\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The Key Management Service customer master key (CMK) to be used for encrypting the batch build output artifacts.</p> <note> <p>You can use a cross-account KMS key to encrypt the build output artifacts if your service role has permission to that key. </p> </note> <p>You can specify either the Amazon Resource Name (ARN) of the CMK or, if available, the CMK's alias (using the format <code>alias/&lt;alias-name&gt;</code>).</p>\"\n        }\n      ]\n    },\n    \"buildBatchNumber\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/WrapperLong\"\n        },\n        {\n          \"description\": \"The number of the batch build. For each project, the <code>buildBatchNumber</code> of its first batch build is <code>1</code>. The <code>buildBatchNumber</code> of each subsequent batch build is incremented by <code>1</code>. If a batch build is deleted, the <code>buildBatchNumber</code> of other batch builds does not change.\"\n        }\n      ]\n    },\n    \"fileSystemLocations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectFileSystemLocations\"\n        },\n        {\n          \"description\": \"An array of <code>ProjectFileSystemLocation</code> objects for the batch build project. A <code>ProjectFileSystemLocation</code> object specifies the <code>identifier</code>, <code>location</code>, <code>mountOptions</code>, <code>mountPoint</code>, and <code>type</code> of a file system created using Amazon Elastic File System.\
  \ \"\n        }\n      ]\n    },\n    \"buildBatchConfig\": {\n      \"$ref\": \"#/components/schemas/ProjectBuildBatchConfig\"\n    },\n    \"buildGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildGroups\"\n        },\n        {\n          \"description\": \"An array of <code>BuildGroup</code> objects that define the build groups for the batch build.\"\n        }\n      ]\n    },\n    \"debugSessionEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \"Specifies if session debugging is enabled for this batch build. For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/session-manager.html\\\">Viewing a running build in Session Manager</a>. Batch session debugging is not supported for matrix batch builds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-batch-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildBatch
---
