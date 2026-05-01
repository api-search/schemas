---
description: Information about the build environment of the build project.
layout: schema
name: ProjectEnvironment
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: image
  type: object
- description: ''
  name: computeType
  type: object
- description: ''
  name: environmentVariables
  type: object
- description: ''
  name: privilegedMode
  type: object
- description: ''
  name: certificate
  type: object
- description: ''
  name: registryCredential
  type: object
- description: ''
  name: imagePullCredentialsType
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-project-environment-schema.json
slug: amazon-codebuild-project-environment
source_filename: amazon-codebuild-project-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-environment-schema.json\",\n  \"title\": \"ProjectEnvironment\",\n  \"description\": \"Information about the build environment of the build project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentType\"\n        },\n        {\n          \"description\": \"<p>The type of build environment to use for related builds.</p> <ul> <li> <p>The environment type <code>ARM_CONTAINER</code> is available only in regions US East (N. Virginia), US East (Ohio), US West (Oregon), EU (Ireland), Asia Pacific (Mumbai), Asia Pacific (Tokyo), Asia Pacific (Sydney), and EU (Frankfurt).</p> </li> <li> <p>The environment type <code>LINUX_CONTAINER</code> with compute type <code>build.general1.2xlarge</code>\
  \ is available only in regions US East (N. Virginia), US East (Ohio), US West (Oregon), Canada (Central), EU (Ireland), EU (London), EU (Frankfurt), Asia Pacific (Tokyo), Asia Pacific (Seoul), Asia Pacific (Singapore), Asia Pacific (Sydney), China (Beijing), and China (Ningxia).</p> </li> <li> <p>The environment type <code>LINUX_GPU_CONTAINER</code> is available only in regions US East (N. Virginia), US East (Ohio), US West (Oregon), Canada (Central), EU (Ireland), EU (London), EU (Frankfurt), Asia Pacific (Tokyo), Asia Pacific (Seoul), Asia Pacific (Singapore), Asia Pacific (Sydney) , China (Beijing), and China (Ningxia).</p> </li> </ul> <ul> <li> <p>The environment types <code>WINDOWS_CONTAINER</code> and <code>WINDOWS_SERVER_2019_CONTAINER</code> are available only in regions US East (N. Virginia), US East (Ohio), US West (Oregon), and EU (Ireland).</p> </li> </ul> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/build-env-ref-compute-types.html\\\
  \">Build environment compute types</a> in the <i>CodeBuild user guide</i>.</p>\"\n        }\n      ]\n    },\n    \"image\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The image tag or image digest that identifies the Docker image to use for this build project. Use the following formats:</p> <ul> <li> <p>For an image tag: <code>&lt;registry&gt;/&lt;repository&gt;:&lt;tag&gt;</code>. For example, in the Docker repository that CodeBuild uses to manage its Docker images, this would be <code>aws/codebuild/standard:4.0</code>. </p> </li> <li> <p>For an image digest: <code>&lt;registry&gt;/&lt;repository&gt;@&lt;digest&gt;</code>. For example, to specify an image with the digest \\\"sha256:cbbf2f9a99b47fc460d422812b6a5adff7dfee951d8fa2e4a98caa0382cfbdbf,\\\" use <code>&lt;registry&gt;/&lt;repository&gt;@sha256:cbbf2f9a99b47fc460d422812b6a5adff7dfee951d8fa2e4a98caa0382cfbdbf</code>.</p>\
  \ </li> </ul> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/build-env-ref-available.html\\\">Docker images provided by CodeBuild</a> in the <i>CodeBuild user guide</i>.</p>\"\n        }\n      ]\n    },\n    \"computeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeType\"\n        },\n        {\n          \"description\": \"<p>Information about the compute resources the build project uses. Available values include:</p> <ul> <li> <p> <code>BUILD_GENERAL1_SMALL</code>: Use up to 3 GB memory and 2 vCPUs for builds.</p> </li> <li> <p> <code>BUILD_GENERAL1_MEDIUM</code>: Use up to 7 GB memory and 4 vCPUs for builds.</p> </li> <li> <p> <code>BUILD_GENERAL1_LARGE</code>: Use up to 16 GB memory and 8 vCPUs for builds, depending on your environment type.</p> </li> <li> <p> <code>BUILD_GENERAL1_2XLARGE</code>: Use up to 145 GB memory, 72 vCPUs, and 824 GB of SSD storage for builds. This compute type supports\
  \ Docker images up to 100 GB uncompressed.</p> </li> </ul> <p> If you use <code>BUILD_GENERAL1_LARGE</code>: </p> <ul> <li> <p> For environment type <code>LINUX_CONTAINER</code>, you can use up to 15 GB memory and 8 vCPUs for builds. </p> </li> <li> <p> For environment type <code>LINUX_GPU_CONTAINER</code>, you can use up to 255 GB memory, 32 vCPUs, and 4 NVIDIA Tesla V100 GPUs for builds.</p> </li> <li> <p> For environment type <code>ARM_CONTAINER</code>, you can use up to 16 GB memory and 8 vCPUs on ARM-based processors for builds.</p> </li> </ul> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/build-env-ref-compute-types.html\\\">Build Environment Compute Types</a> in the <i>CodeBuild User Guide.</i> </p>\"\n        }\n      ]\n    },\n    \"environmentVariables\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentVariables\"\n        },\n        {\n          \"description\": \"A set of environment\
  \ variables to make available to builds for this build project.\"\n        }\n      ]\n    },\n    \"privilegedMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \"<p>Enables running the Docker daemon inside a Docker container. Set to true only if the build project is used to build Docker images. Otherwise, a build that attempts to interact with the Docker daemon fails. The default setting is <code>false</code>.</p> <p>You can initialize the Docker daemon during the install phase of your build by adding one of the following sets of commands to the install phase of your buildspec file:</p> <p>If the operating system's base image is Ubuntu Linux:</p> <p> <code>- nohup /usr/local/bin/dockerd --host=unix:///var/run/docker.sock --host=tcp://0.0.0.0:2375 --storage-driver=overlay&amp;</code> </p> <p> <code>- timeout 15 sh -c \\\"until docker info; do echo .; sleep 1; done\\\"</code> </p> <p>If\
  \ the operating system's base image is Alpine Linux and the previous command does not work, add the <code>-t</code> argument to <code>timeout</code>:</p> <p> <code>- nohup /usr/local/bin/dockerd --host=unix:///var/run/docker.sock --host=tcp://0.0.0.0:2375 --storage-driver=overlay&amp;</code> </p> <p> <code>- timeout -t 15 sh -c \\\"until docker info; do echo .; sleep 1; done\\\"</code> </p>\"\n        }\n      ]\n    },\n    \"certificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN of the Amazon S3 bucket, path prefix, and object key that contains the PEM-encoded certificate for the build project. For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/create-project-cli.html#cli.environment.certificate\\\">certificate</a> in the <i>CodeBuild User Guide</i>.\"\n        }\n      ]\n    },\n    \"registryCredential\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/RegistryCredential\"\n        },\n        {\n          \"description\": \" The credentials for access to a private registry.\"\n        }\n      ]\n    },\n    \"imagePullCredentialsType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImagePullCredentialsType\"\n        },\n        {\n          \"description\": \"<p> The type of credentials CodeBuild uses to pull images in your build. There are two valid values: </p> <ul> <li> <p> <code>CODEBUILD</code> specifies that CodeBuild uses its own credentials. This requires that you modify your ECR repository policy to trust CodeBuild service principal. </p> </li> <li> <p> <code>SERVICE_ROLE</code> specifies that CodeBuild uses your build project's service role. </p> </li> </ul> <p> When you use a cross-account or private registry image, you must use SERVICE_ROLE credentials. When you use an CodeBuild curated image, you must use CODEBUILD credentials. </p>\"\n \
  \       }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"image\",\n    \"computeType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-environment-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ProjectEnvironment
---
