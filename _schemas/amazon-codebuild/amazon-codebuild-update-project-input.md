---
description: UpdateProjectInput schema from Amazon CodeBuild
layout: schema
name: UpdateProjectInput
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: source
  type: object
- description: ''
  name: secondarySources
  type: object
- description: ''
  name: sourceVersion
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
  name: timeoutInMinutes
  type: object
- description: ''
  name: queuedTimeoutInMinutes
  type: object
- description: ''
  name: encryptionKey
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: vpcConfig
  type: object
- description: ''
  name: badgeEnabled
  type: object
- description: ''
  name: logsConfig
  type: object
- description: ''
  name: fileSystemLocations
  type: object
- description: ''
  name: buildBatchConfig
  type: object
- description: ''
  name: concurrentBuildLimit
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-update-project-input-schema.json
slug: amazon-codebuild-update-project-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-project-input-schema.json\",\n  \"title\": \"UpdateProjectInput\",\n  \"description\": \"UpdateProjectInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The name of the build project.</p> <note> <p>You cannot change a build project's name.</p> </note>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectDescription\"\n        },\n        {\n          \"description\": \"A new or replacement description of the build project.\"\n        }\n      ]\n    },\n    \"source\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/ProjectSource\"\n        },\n        {\n          \"description\": \"Information to be changed about the build input source code for the build project.\"\n        }\n      ]\n    },\n    \"secondarySources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectSources\"\n        },\n        {\n          \"description\": \" An array of <code>ProjectSource</code> objects. \"\n        }\n      ]\n    },\n    \"sourceVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p> A version of the build input to be built for this project. If not specified, the latest version is used. If specified, it must be one of: </p> <ul> <li> <p>For CodeCommit: the commit ID, branch, or Git tag to use.</p> </li> <li> <p>For GitHub: the commit ID, pull request ID, branch name, or tag name that corresponds to the version of the source code you\
  \ want to build. If a pull request ID is specified, it must use the format <code>pr/pull-request-ID</code> (for example <code>pr/25</code>). If a branch name is specified, the branch's HEAD commit ID is used. If not specified, the default branch's HEAD commit ID is used.</p> </li> <li> <p>For Bitbucket: the commit ID, branch name, or tag name that corresponds to the version of the source code you want to build. If a branch name is specified, the branch's HEAD commit ID is used. If not specified, the default branch's HEAD commit ID is used.</p> </li> <li> <p>For Amazon S3: the version ID of the object that represents the build input ZIP file to use.</p> </li> </ul> <p> If <code>sourceVersion</code> is specified at the build level, then that version takes precedence over this <code>sourceVersion</code> (at the project level). </p> <p> For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/sample-source-version.html\\\">Source Version Sample with CodeBuild</a>\
  \ in the <i>CodeBuild User Guide</i>. </p>\"\n        }\n      ]\n    },\n    \"secondarySourceVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectSecondarySourceVersions\"\n        },\n        {\n          \"description\": \" An array of <code>ProjectSourceVersion</code> objects. If <code>secondarySourceVersions</code> is specified at the build level, then they take over these <code>secondarySourceVersions</code> (at the project level). \"\n        }\n      ]\n    },\n    \"artifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectArtifacts\"\n        },\n        {\n          \"description\": \"Information to be changed about the build output artifacts for the build project.\"\n        }\n      ]\n    },\n    \"secondaryArtifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectArtifactsList\"\n        },\n        {\n          \"description\": \" An array of <code>ProjectArtifact</code>\
  \ objects. \"\n        }\n      ]\n    },\n    \"cache\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectCache\"\n        },\n        {\n          \"description\": \"Stores recently used information so that it can be quickly accessed at a later time.\"\n        }\n      ]\n    },\n    \"environment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectEnvironment\"\n        },\n        {\n          \"description\": \"Information to be changed about the build environment for the build project.\"\n        }\n      ]\n    },\n    \"serviceRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The replacement ARN of the IAM role that enables CodeBuild to interact with dependent Amazon Web Services services on behalf of the Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"timeoutInMinutes\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/TimeOut\"\n        },\n        {\n          \"description\": \"The replacement value in minutes, from 5 to 480 (8 hours), for CodeBuild to wait before timing out any related build that did not get marked as completed.\"\n        }\n      ]\n    },\n    \"queuedTimeoutInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeOut\"\n        },\n        {\n          \"description\": \" The number of minutes a build is allowed to be queued before it times out. \"\n        }\n      ]\n    },\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The Key Management Service customer master key (CMK) to be used for encrypting the build output artifacts.</p> <note> <p> You can use a cross-account KMS key to encrypt the build output artifacts if your service role has permission to that\
  \ key. </p> </note> <p>You can specify either the Amazon Resource Name (ARN) of the CMK or, if available, the CMK's alias (using the format <code>alias/&lt;alias-name&gt;</code>). </p>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>An updated list of tag key and value pairs associated with this build project.</p> <p>These tags are available for use by Amazon Web Services services that support CodeBuild build project tags.</p>\"\n        }\n      ]\n    },\n    \"vpcConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfig\"\n        },\n        {\n          \"description\": \"VpcConfig enables CodeBuild to access resources in an Amazon VPC.\"\n        }\n      ]\n    },\n    \"badgeEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n\
  \          \"description\": \"Set this to true to generate a publicly accessible URL for your project's build badge.\"\n        }\n      ]\n    },\n    \"logsConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogsConfig\"\n        },\n        {\n          \"description\": \" Information about logs for the build project. A project can create logs in CloudWatch Logs, logs in an S3 bucket, or both. \"\n        }\n      ]\n    },\n    \"fileSystemLocations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectFileSystemLocations\"\n        },\n        {\n          \"description\": \" An array of <code>ProjectFileSystemLocation</code> objects for a CodeBuild build project. A <code>ProjectFileSystemLocation</code> object specifies the <code>identifier</code>, <code>location</code>, <code>mountOptions</code>, <code>mountPoint</code>, and <code>type</code> of a file system created using Amazon Elastic File System. \"\n      \
  \  }\n      ]\n    },\n    \"buildBatchConfig\": {\n      \"$ref\": \"#/components/schemas/ProjectBuildBatchConfig\"\n    },\n    \"concurrentBuildLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperInt\"\n        },\n        {\n          \"description\": \"<p>The maximum number of concurrent builds that are allowed for this project.</p> <p>New builds are only started if the current number of builds is less than or equal to this limit. If the current build count meets this limit, new builds are throttled and are not run.</p> <p>To remove this limit, set this value to -1.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-project-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: UpdateProjectInput
---
