---
description: Information about build output artifacts.
layout: schema
name: BuildArtifacts
properties_list:
- description: ''
  name: location
  type: object
- description: ''
  name: sha256sum
  type: object
- description: ''
  name: md5sum
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
schema_file: json-schema/amazon-codebuild-build-artifacts-schema.json
slug: amazon-codebuild-build-artifacts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-artifacts-schema.json\",\n  \"title\": \"BuildArtifacts\",\n  \"description\": \"Information about build output artifacts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Information about the location of the build artifacts.\"\n        }\n      ]\n    },\n    \"sha256sum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The SHA-256 hash of the build artifact.</p> <p>You can use this hash along with a checksum tool to confirm file integrity and authenticity.</p> <note> <p>This value is available only if the build project's <code>packaging</code>\
  \ value is set to <code>ZIP</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"md5sum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The MD5 hash of the build artifact.</p> <p>You can use this hash along with a checksum tool to confirm file integrity and authenticity.</p> <note> <p>This value is available only if the build project's <code>packaging</code> value is set to <code>ZIP</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"overrideArtifactName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \" If this flag is set, a name specified in the buildspec file overrides the artifact name. The name specified in a buildspec file is calculated at build time and uses the Shell Command Language. For example, you can append a date and time to your artifact name so that it is always unique.\
  \ \"\n        }\n      ]\n    },\n    \"encryptionDisabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \" Information that tells you if encryption for build artifacts is disabled. \"\n        }\n      ]\n    },\n    \"artifactIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" An identifier for this artifact definition. \"\n        }\n      ]\n    },\n    \"bucketOwnerAccess\": {\n      \"$ref\": \"#/components/schemas/BucketOwnerAccess\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-artifacts-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildArtifacts
---
