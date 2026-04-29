---
description: Represents a build or deployment notification sent to the Bugsnag Build API, containing version information, source control details, and optional metadata.
layout: schema
name: Bugsnag Build
properties_list:
- description: The Bugsnag API key for the project.
  name: apiKey
  type: string
- description: The version of the application being built or deployed.
  name: appVersion
  type: string
- description: The version code of the application, typically used for Android applications.
  name: appVersionCode
  type: string
- description: The bundle version of the application, typically used for iOS applications.
  name: appBundleVersion
  type: string
- description: The release stage for this build (e.g., production, staging, development).
  name: releaseStage
  type: string
- description: The name of the person or system that created this build.
  name: builderName
  type: string
- description: ''
  name: sourceControl
  type: object
- description: Custom metadata to associate with the build.
  name: metadata
  type: object
- description: Whether to automatically assign this build as a release.
  name: autoAssignRelease
  type: boolean
provider_name: bugsnag
provider_slug: bugsnag
schema_file: json-schema/bugsnag-build-schema.json
slug: bugsnag-build
source_filename: bugsnag-build-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://bugsnag.com/schemas/bugsnag/build.json\",\n  \"title\": \"Bugsnag Build\",\n  \"description\": \"Represents a build or deployment notification sent to the Bugsnag Build API, containing version information, source control details, and optional metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"apiKey\", \"appVersion\"],\n  \"properties\": {\n    \"apiKey\": {\n      \"type\": \"string\",\n      \"description\": \"The Bugsnag API key for the project.\",\n      \"pattern\": \"^[a-f0-9]{32}$\"\n    },\n    \"appVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the application being built or deployed.\",\n      \"minLength\": 1\n    },\n    \"appVersionCode\": {\n      \"type\": \"string\",\n      \"description\": \"The version code of the application, typically used for Android applications.\"\n    },\n    \"appBundleVersion\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The bundle version of the application, typically used for iOS applications.\"\n    },\n    \"releaseStage\": {\n      \"type\": \"string\",\n      \"description\": \"The release stage for this build (e.g., production, staging, development).\",\n      \"default\": \"production\"\n    },\n    \"builderName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the person or system that created this build.\"\n    },\n    \"sourceControl\": {\n      \"$ref\": \"#/$defs/SourceControl\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata to associate with the build.\",\n      \"additionalProperties\": true\n    },\n    \"autoAssignRelease\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to automatically assign this build as a release.\",\n      \"default\": true\n    }\n  },\n  \"$defs\": {\n    \"SourceControl\": {\n      \"type\": \"object\",\n      \"description\": \"Source\
  \ control information for the build, linking errors to specific commits and repositories.\",\n      \"properties\": {\n        \"provider\": {\n          \"type\": \"string\",\n          \"description\": \"The source control provider name.\",\n          \"enum\": [\n            \"github\",\n            \"github-enterprise\",\n            \"gitlab\",\n            \"gitlab-onpremise\",\n            \"bitbucket\",\n            \"bitbucket-server\"\n          ]\n        },\n        \"repository\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the source control repository.\"\n        },\n        \"revision\": {\n          \"type\": \"string\",\n          \"description\": \"The source control revision or commit hash for this build.\"\n        },\n        \"diff\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A URL to the diff between this build and the previous one.\"\n        }\n\
  \      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/json-schema/bugsnag-build-schema.json
tags: []
title: Bugsnag Build
---
