---
description: Information about the cache for the build project.
layout: schema
name: ProjectCache
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: modes
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-project-cache-schema.json
slug: amazon-codebuild-project-cache
source_filename: amazon-codebuild-project-cache-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-cache-schema.json\",\n  \"title\": \"ProjectCache\",\n  \"description\": \"Information about the cache for the build project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CacheType\"\n        },\n        {\n          \"description\": \"<p>The type of cache used by the build project. Valid values include:</p> <ul> <li> <p> <code>NO_CACHE</code>: The build project does not use any cache.</p> </li> <li> <p> <code>S3</code>: The build project reads and writes from and to S3.</p> </li> <li> <p> <code>LOCAL</code>: The build project stores a cache locally on a build host that is only available to that build host.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"location\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Information about the cache location: </p> <ul> <li> <p> <code>NO_CACHE</code> or <code>LOCAL</code>: This value is ignored.</p> </li> <li> <p> <code>S3</code>: This is the S3 bucket name/prefix.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"modes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectCacheModes\"\n        },\n        {\n          \"description\": \"<p>An array of strings that specify the local cache modes. You can use one or more local cache modes at the same time. This is only used for <code>LOCAL</code> cache types.</p> <p>Possible values are:</p> <dl> <dt>LOCAL_SOURCE_CACHE</dt> <dd> <p>Caches Git metadata for primary and secondary sources. After the cache is created, subsequent builds pull only the change between commits. This mode is a good choice for projects with a clean working directory and a\
  \ source that is a large Git repository. If you choose this option and your project does not use a Git repository (GitHub, GitHub Enterprise, or Bitbucket), the option is ignored. </p> </dd> <dt>LOCAL_DOCKER_LAYER_CACHE</dt> <dd> <p>Caches existing Docker layers. This mode is a good choice for projects that build or pull large Docker images. It can prevent the performance issues caused by pulling large Docker images down from the network. </p> <note> <ul> <li> <p>You can use a Docker layer cache in the Linux environment only. </p> </li> <li> <p>The <code>privileged</code> flag must be set so that your project has the required Docker permissions. </p> </li> <li> <p>You should consider the security implications before you use a Docker layer cache. </p> </li> </ul> </note> </dd> <dt>LOCAL_CUSTOM_CACHE</dt> <dd> <p>Caches directories you specify in the buildspec file. This mode is a good choice if your build scenario is not suited to one of the other three local cache modes. If you use a custom\
  \ cache: </p> <ul> <li> <p>Only directories can be specified for caching. You cannot specify individual files. </p> </li> <li> <p>Symlinks are used to reference cached directories. </p> </li> <li> <p>Cached directories are linked to your build before it downloads its project sources. Cached items are overridden if a source item has the same name. Directories are specified using cache paths in the buildspec file. </p> </li> </ul> </dd> </dl>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-cache-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ProjectCache
---
