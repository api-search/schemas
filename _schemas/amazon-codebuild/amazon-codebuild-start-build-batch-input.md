---
description: StartBuildBatchInput schema from Amazon CodeBuild
layout: schema
name: StartBuildBatchInput
properties_list:
- description: ''
  name: projectName
  type: object
- description: ''
  name: secondarySourcesOverride
  type: object
- description: ''
  name: secondarySourcesVersionOverride
  type: object
- description: ''
  name: sourceVersion
  type: object
- description: ''
  name: artifactsOverride
  type: object
- description: ''
  name: secondaryArtifactsOverride
  type: object
- description: ''
  name: environmentVariablesOverride
  type: object
- description: ''
  name: sourceTypeOverride
  type: object
- description: ''
  name: sourceLocationOverride
  type: object
- description: ''
  name: sourceAuthOverride
  type: object
- description: ''
  name: gitCloneDepthOverride
  type: object
- description: ''
  name: gitSubmodulesConfigOverride
  type: object
- description: ''
  name: buildspecOverride
  type: object
- description: ''
  name: insecureSslOverride
  type: object
- description: ''
  name: reportBuildBatchStatusOverride
  type: object
- description: ''
  name: environmentTypeOverride
  type: object
- description: ''
  name: imageOverride
  type: object
- description: ''
  name: computeTypeOverride
  type: object
- description: ''
  name: certificateOverride
  type: object
- description: ''
  name: cacheOverride
  type: object
- description: ''
  name: serviceRoleOverride
  type: object
- description: ''
  name: privilegedModeOverride
  type: object
- description: ''
  name: buildTimeoutInMinutesOverride
  type: object
- description: ''
  name: queuedTimeoutInMinutesOverride
  type: object
- description: ''
  name: encryptionKeyOverride
  type: object
- description: ''
  name: logsConfigOverride
  type: object
- description: ''
  name: registryCredentialOverride
  type: object
- description: ''
  name: imagePullCredentialsTypeOverride
  type: object
- description: ''
  name: buildBatchConfigOverride
  type: object
- description: ''
  name: debugSessionEnabled
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-start-build-batch-input-schema.json
slug: amazon-codebuild-start-build-batch-input
source_filename: amazon-codebuild-start-build-batch-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-start-build-batch-input-schema.json\",\n  \"title\": \"StartBuildBatchInput\",\n  \"description\": \"StartBuildBatchInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the project.\"\n        }\n      ]\n    },\n    \"secondarySourcesOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectSources\"\n        },\n        {\n          \"description\": \"An array of <code>ProjectSource</code> objects that override the secondary sources defined in the batch build project.\"\n        }\n      ]\n    },\n    \"secondarySourcesVersionOverride\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectSecondarySourceVersions\"\n        },\n        {\n          \"description\": \"An array of <code>ProjectSourceVersion</code> objects that override the secondary source versions in the batch build project.\"\n        }\n      ]\n    },\n    \"sourceVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The version of the batch build input to be built, for this build only. If not specified, the latest version is used. If specified, the contents depends on the source provider:</p> <dl> <dt>CodeCommit</dt> <dd> <p>The commit ID, branch, or Git tag to use.</p> </dd> <dt>GitHub</dt> <dd> <p>The commit ID, pull request ID, branch name, or tag name that corresponds to the version of the source code you want to build. If a pull request ID is specified, it must use the format <code>pr/pull-request-ID</code> (for example\
  \ <code>pr/25</code>). If a branch name is specified, the branch's HEAD commit ID is used. If not specified, the default branch's HEAD commit ID is used.</p> </dd> <dt>Bitbucket</dt> <dd> <p>The commit ID, branch name, or tag name that corresponds to the version of the source code you want to build. If a branch name is specified, the branch's HEAD commit ID is used. If not specified, the default branch's HEAD commit ID is used.</p> </dd> <dt>Amazon S3</dt> <dd> <p>The version ID of the object that represents the build input ZIP file to use.</p> </dd> </dl> <p>If <code>sourceVersion</code> is specified at the project level, then this <code>sourceVersion</code> (at the build level) takes precedence. </p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/sample-source-version.html\\\">Source Version Sample with CodeBuild</a> in the <i>CodeBuild User Guide</i>. </p>\"\n        }\n      ]\n    },\n    \"artifactsOverride\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/ProjectArtifacts\"\n        },\n        {\n          \"description\": \"An array of <code>ProjectArtifacts</code> objects that contains information about the build output artifact overrides for the build project.\"\n        }\n      ]\n    },\n    \"secondaryArtifactsOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectArtifactsList\"\n        },\n        {\n          \"description\": \"An array of <code>ProjectArtifacts</code> objects that override the secondary artifacts defined in the batch build project.\"\n        }\n      ]\n    },\n    \"environmentVariablesOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentVariables\"\n        },\n        {\n          \"description\": \"An array of <code>EnvironmentVariable</code> objects that override, or add to, the environment variables defined in the batch build project.\"\n        }\n      ]\n \
  \   },\n    \"sourceTypeOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceType\"\n        },\n        {\n          \"description\": \"The source input type that overrides the source input defined in the batch build project.\"\n        }\n      ]\n    },\n    \"sourceLocationOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A location that overrides, for this batch build, the source location defined in the batch build project.\"\n        }\n      ]\n    },\n    \"sourceAuthOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceAuth\"\n        },\n        {\n          \"description\": \"A <code>SourceAuth</code> object that overrides the one defined in the batch build project. This override applies only if the build project's source is BitBucket or GitHub.\"\n        }\n      ]\n    },\n    \"gitCloneDepthOverride\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitCloneDepth\"\n        },\n        {\n          \"description\": \"The user-defined depth of history, with a minimum value of 0, that overrides, for this batch build only, any previous depth of history defined in the batch build project.\"\n        }\n      ]\n    },\n    \"gitSubmodulesConfigOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitSubmodulesConfig\"\n        },\n        {\n          \"description\": \"A <code>GitSubmodulesConfig</code> object that overrides the Git submodules configuration for this batch build.\"\n        }\n      ]\n    },\n    \"buildspecOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>A buildspec file declaration that overrides, for this build only, the latest one already defined in the build project.</p> <p>If this value is set, it\
  \ can be either an inline buildspec definition, the path to an alternate buildspec file relative to the value of the built-in <code>CODEBUILD_SRC_DIR</code> environment variable, or the path to an S3 bucket. The bucket must be in the same Amazon Web Services Region as the build project. Specify the buildspec file using its ARN (for example, <code>arn:aws:s3:::my-codebuild-sample2/buildspec.yml</code>). If this value is not provided or is set to an empty string, the source code must contain a buildspec file in its root directory. For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/build-spec-ref.html#build-spec-ref-name-storage\\\">Buildspec File Name and Storage Location</a>. </p>\"\n        }\n      ]\n    },\n    \"insecureSslOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \"Enable this flag to override the insecure SSL setting that is\
  \ specified in the batch build project. The insecure SSL setting determines whether to ignore SSL warnings while connecting to the project source code. This override applies only if the build's source is GitHub Enterprise.\"\n        }\n      ]\n    },\n    \"reportBuildBatchStatusOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \"<p>Set to <code>true</code> to report to your source provider the status of a batch build's start and completion. If you use this option with a source provider other than GitHub, GitHub Enterprise, or Bitbucket, an <code>invalidInputException</code> is thrown. </p> <note> <p>The status of a build triggered by a webhook is always reported to your source provider. </p> </note>\"\n        }\n      ]\n    },\n    \"environmentTypeOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentType\"\n        },\n        {\n\
  \          \"description\": \"A container type for this batch build that overrides the one specified in the batch build project.\"\n        }\n      ]\n    },\n    \"imageOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of an image for this batch build that overrides the one specified in the batch build project.\"\n        }\n      ]\n    },\n    \"computeTypeOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeType\"\n        },\n        {\n          \"description\": \"The name of a compute type for this batch build that overrides the one specified in the batch build project.\"\n        }\n      ]\n    },\n    \"certificateOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of a certificate for this batch build that overrides\
  \ the one specified in the batch build project.\"\n        }\n      ]\n    },\n    \"cacheOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectCache\"\n        },\n        {\n          \"description\": \"A <code>ProjectCache</code> object that specifies cache overrides.\"\n        }\n      ]\n    },\n    \"serviceRoleOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of a service role for this batch build that overrides the one specified in the batch build project.\"\n        }\n      ]\n    },\n    \"privilegedModeOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \"Enable this flag to override privileged mode in the batch build project.\"\n        }\n      ]\n    },\n    \"buildTimeoutInMinutesOverride\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/TimeOut\"\n        },\n        {\n          \"description\": \"Overrides the build timeout specified in the batch build project.\"\n        }\n      ]\n    },\n    \"queuedTimeoutInMinutesOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeOut\"\n        },\n        {\n          \"description\": \"The number of minutes a batch build is allowed to be queued before it times out.\"\n        }\n      ]\n    },\n    \"encryptionKeyOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The Key Management Service customer master key (CMK) that overrides the one specified in the batch build project. The CMK key encrypts the build output artifacts.</p> <note> <p>You can use a cross-account KMS key to encrypt the build output artifacts if your service role has permission to that key. </p> </note>\
  \ <p>You can specify either the Amazon Resource Name (ARN) of the CMK or, if available, the CMK's alias (using the format <code>alias/&lt;alias-name&gt;</code>).</p>\"\n        }\n      ]\n    },\n    \"logsConfigOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogsConfig\"\n        },\n        {\n          \"description\": \"A <code>LogsConfig</code> object that override the log settings defined in the batch build project.\"\n        }\n      ]\n    },\n    \"registryCredentialOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistryCredential\"\n        },\n        {\n          \"description\": \"A <code>RegistryCredential</code> object that overrides credentials for access to a private registry.\"\n        }\n      ]\n    },\n    \"imagePullCredentialsTypeOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImagePullCredentialsType\"\n        },\n        {\n          \"\
  description\": \"<p>The type of credentials CodeBuild uses to pull images in your batch build. There are two valid values: </p> <dl> <dt>CODEBUILD</dt> <dd> <p>Specifies that CodeBuild uses its own credentials. This requires that you modify your ECR repository policy to trust CodeBuild's service principal.</p> </dd> <dt>SERVICE_ROLE</dt> <dd> <p>Specifies that CodeBuild uses your build project's service role. </p> </dd> </dl> <p>When using a cross-account or private registry image, you must use <code>SERVICE_ROLE</code> credentials. When using an CodeBuild curated image, you must use <code>CODEBUILD</code> credentials. </p>\"\n        }\n      ]\n    },\n    \"buildBatchConfigOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectBuildBatchConfig\"\n        },\n        {\n          \"description\": \"A <code>BuildBatchConfigOverride</code> object that contains batch build configuration overrides.\"\n        }\n      ]\n    },\n    \"debugSessionEnabled\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \"Specifies if session debugging is enabled for this batch build. For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/session-manager.html\\\">Viewing a running build in Session Manager</a>. Batch session debugging is not supported for matrix batch builds.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projectName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-start-build-batch-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: StartBuildBatchInput
---
