---
description: A CircleCI pipeline represents a full CI/CD execution triggered by a code change, API call, or schedule. It contains one or more workflows that organize and run jobs.
layout: schema
name: CircleCI Pipeline
properties_list:
- description: The unique identifier of the pipeline
  name: id
  type: string
- description: Errors that occurred during pipeline setup
  name: errors
  type: array
- description: The project slug in vcs-slug/org-name/repo-name format
  name: project_slug
  type: string
- description: When the pipeline was last updated
  name: updated_at
  type: string
- description: The monotonically increasing pipeline number
  name: number
  type: integer
- description: The current state of the pipeline
  name: state
  type: string
- description: When the pipeline was created
  name: created_at
  type: string
- description: ''
  name: trigger
  type: object
- description: Parameters passed when triggering the pipeline
  name: trigger_parameters
  type: object
- description: ''
  name: vcs
  type: object
provider_name: CircleCI
provider_slug: circleci
schema_file: json-schema/circleci-pipeline-schema.json
slug: circleci-pipeline
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
title: CircleCI Pipeline
---
