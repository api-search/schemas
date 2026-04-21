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
tags: []
title: Bugsnag Build
---
