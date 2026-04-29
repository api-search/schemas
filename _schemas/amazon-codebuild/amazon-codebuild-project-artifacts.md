---
description: Information about the build output artifacts for the build project.
layout: schema
name: ProjectArtifacts
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: path
  type: object
- description: ''
  name: namespaceType
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: packaging
  type: object
- description: ''
  name: overrideArtifactName
  type: object
- description: ''
  name: encryptionDisabled
  type: object
- description: ''
  name: artifactIdentifier
  type: object
- description: ''
  name: bucketOwnerAccess
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-project-artifacts-schema.json
slug: amazon-codebuild-project-artifacts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-artifacts-schema.json\",\n  \"title\": \"ProjectArtifacts\",\n  \"description\": \"Information about the build output artifacts for the build project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactsType\"\n        },\n        {\n          \"description\": \"<p>The type of build output artifact. Valid values include:</p> <ul> <li> <p> <code>CODEPIPELINE</code>: The build project has build output generated through CodePipeline. </p> <note> <p>The <code>CODEPIPELINE</code> type is not supported for <code>secondaryArtifacts</code>.</p> </note> </li> <li> <p> <code>NO_ARTIFACTS</code>: The build project does not produce any build output.</p> </li> <li> <p> <code>S3</code>: The build\
  \ project stores build output in Amazon S3.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Information about the build output artifact location:</p> <ul> <li> <p>If <code>type</code> is set to <code>CODEPIPELINE</code>, CodePipeline ignores this value if specified. This is because CodePipeline manages its build output locations instead of CodeBuild.</p> </li> <li> <p>If <code>type</code> is set to <code>NO_ARTIFACTS</code>, this value is ignored if specified, because no build output is produced.</p> </li> <li> <p>If <code>type</code> is set to <code>S3</code>, this is the name of the output bucket.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Along with <code>namespaceType</code>\
  \ and <code>name</code>, the pattern that CodeBuild uses to name and store the output artifact:</p> <ul> <li> <p>If <code>type</code> is set to <code>CODEPIPELINE</code>, CodePipeline ignores this value if specified. This is because CodePipeline manages its build output names instead of CodeBuild.</p> </li> <li> <p>If <code>type</code> is set to <code>NO_ARTIFACTS</code>, this value is ignored if specified, because no build output is produced.</p> </li> <li> <p>If <code>type</code> is set to <code>S3</code>, this is the path to the output artifact. If <code>path</code> is not specified, <code>path</code> is not used.</p> </li> </ul> <p>For example, if <code>path</code> is set to <code>MyArtifacts</code>, <code>namespaceType</code> is set to <code>NONE</code>, and <code>name</code> is set to <code>MyArtifact.zip</code>, the output artifact is stored in the output bucket at <code>MyArtifacts/MyArtifact.zip</code>.</p>\"\n        }\n      ]\n    },\n    \"namespaceType\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactNamespace\"\n        },\n        {\n          \"description\": \"<p>Along with <code>path</code> and <code>name</code>, the pattern that CodeBuild uses to determine the name and location to store the output artifact:</p> <ul> <li> <p>If <code>type</code> is set to <code>CODEPIPELINE</code>, CodePipeline ignores this value if specified. This is because CodePipeline manages its build output names instead of CodeBuild.</p> </li> <li> <p>If <code>type</code> is set to <code>NO_ARTIFACTS</code>, this value is ignored if specified, because no build output is produced.</p> </li> <li> <p>If <code>type</code> is set to <code>S3</code>, valid values include:</p> <ul> <li> <p> <code>BUILD_ID</code>: Include the build ID in the location of the build output artifact.</p> </li> <li> <p> <code>NONE</code>: Do not include the build ID. This is the default if <code>namespaceType</code> is not specified.</p> </li> </ul> </li> </ul> <p>For\
  \ example, if <code>path</code> is set to <code>MyArtifacts</code>, <code>namespaceType</code> is set to <code>BUILD_ID</code>, and <code>name</code> is set to <code>MyArtifact.zip</code>, the output artifact is stored in <code>MyArtifacts/&lt;build-ID&gt;/MyArtifact.zip</code>.</p>\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Along with <code>path</code> and <code>namespaceType</code>, the pattern that CodeBuild uses to name and store the output artifact:</p> <ul> <li> <p>If <code>type</code> is set to <code>CODEPIPELINE</code>, CodePipeline ignores this value if specified. This is because CodePipeline manages its build output names instead of CodeBuild.</p> </li> <li> <p>If <code>type</code> is set to <code>NO_ARTIFACTS</code>, this value is ignored if specified, because no build output is produced.</p> </li> <li> <p>If <code>type</code> is set\
  \ to <code>S3</code>, this is the name of the output artifact object. If you set the name to be a forward slash (\\\"/\\\"), the artifact is stored in the root of the output bucket.</p> </li> </ul> <p>For example:</p> <ul> <li> <p> If <code>path</code> is set to <code>MyArtifacts</code>, <code>namespaceType</code> is set to <code>BUILD_ID</code>, and <code>name</code> is set to <code>MyArtifact.zip</code>, then the output artifact is stored in <code>MyArtifacts/&lt;build-ID&gt;/MyArtifact.zip</code>. </p> </li> <li> <p> If <code>path</code> is empty, <code>namespaceType</code> is set to <code>NONE</code>, and <code>name</code> is set to \\\"<code>/</code>\\\", the output artifact is stored in the root of the output bucket. </p> </li> <li> <p> If <code>path</code> is set to <code>MyArtifacts</code>, <code>namespaceType</code> is set to <code>BUILD_ID</code>, and <code>name</code> is set to \\\"<code>/</code>\\\", the output artifact is stored in <code>MyArtifacts/&lt;build-ID&gt;</code>.\
  \ </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"packaging\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactPackaging\"\n        },\n        {\n          \"description\": \"<p>The type of build output artifact to create:</p> <ul> <li> <p>If <code>type</code> is set to <code>CODEPIPELINE</code>, CodePipeline ignores this value if specified. This is because CodePipeline manages its build output artifacts instead of CodeBuild.</p> </li> <li> <p>If <code>type</code> is set to <code>NO_ARTIFACTS</code>, this value is ignored if specified, because no build output is produced.</p> </li> <li> <p>If <code>type</code> is set to <code>S3</code>, valid values include:</p> <ul> <li> <p> <code>NONE</code>: CodeBuild creates in the output bucket a folder that contains the build output. This is the default if <code>packaging</code> is not specified.</p> </li> <li> <p> <code>ZIP</code>: CodeBuild creates in the output bucket a ZIP file that contains the build\
  \ output.</p> </li> </ul> </li> </ul>\"\n        }\n      ]\n    },\n    \"overrideArtifactName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \" If this flag is set, a name specified in the buildspec file overrides the artifact name. The name specified in a buildspec file is calculated at build time and uses the Shell Command Language. For example, you can append a date and time to your artifact name so that it is always unique. \"\n        }\n      ]\n    },\n    \"encryptionDisabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \" Set to true if you do not want your output artifacts encrypted. This option is valid only if your artifacts type is Amazon S3. If this is set with another artifacts type, an invalidInputException is thrown. \"\n        }\n      ]\n    },\n    \"artifactIdentifier\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" An identifier for this artifact definition. \"\n        }\n      ]\n    },\n    \"bucketOwnerAccess\": {\n      \"$ref\": \"#/components/schemas/BucketOwnerAccess\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-artifacts-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ProjectArtifacts
---
