---
description: Schema for the .all-contributorsrc configuration file used by the All Contributors specification and bot to manage open-source project contributor attribution.
layout: schema
name: AllContributorsConfig
properties_list:
- description: Name of the project repository.
  name: projectName
  type: string
- description: GitHub username or organization that owns the project.
  name: projectOwner
  type: string
- description: Type of repository hosting service.
  name: repoType
  type: string
- description: Hostname of the repository hosting service.
  name: repoHost
  type: string
- description: List of files to update with contributor tables.
  name: files
  type: array
- description: Size in pixels for contributor avatar images.
  name: imageSize
  type: integer
- description: Whether to automatically commit changes when contributors are added.
  name: commit
  type: boolean
- description: Commit message convention to follow.
  name: commitConvention
  type: string
- description: Maximum number of contributors to display per line in the table.
  name: contributorsPerLine
  type: integer
- description: Custom template for the contributors badge markdown.
  name: badgeTemplate
  type: string
- description: Custom template for individual contributor entries in the table.
  name: contributorTemplate
  type: string
- description: Custom contribution type definitions extending the default types.
  name: types
  type: object
- description: List of contributors to the project.
  name: contributors
  type: array
provider_name: AUTHORS.md
provider_slug: authors-md
schema_file: json-schema/all-contributors-config-schema.json
slug: all-contributors-config
tags:
- Attribution
- Documentation
- Open Source
- Repository
- File Format
- Contributor Management
- License Compliance
- Standard
title: AllContributorsConfig
---
