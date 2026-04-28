---
description: A CircleCI workflow organizes a set of jobs and defines the order, dependencies, and conditions under which they run within a pipeline.
layout: schema
name: CircleCI Workflow
properties_list:
- description: The unique identifier of the pipeline this workflow belongs to
  name: pipeline_id
  type: string
- description: The unique identifier of the workflow
  name: id
  type: string
- description: The name of the workflow as defined in the CircleCI configuration
  name: name
  type: string
- description: The project slug in vcs-slug/org-name/repo-name format
  name: project_slug
  type: string
- description: The current status of the workflow
  name: status
  type: string
- description: The ID of the user who started the workflow
  name: started_by
  type: string
- description: The pipeline number
  name: pipeline_number
  type: integer
- description: When the workflow was created
  name: created_at
  type: string
- description: When the workflow stopped, null if still running
  name: stopped_at
  type:
  - string
  - 'null'
- description: Tag for special workflow types like setup workflows
  name: tag
  type: string
provider_name: CircleCI
provider_slug: circleci
schema_file: json-schema/circleci-workflow-schema.json
slug: circleci-workflow
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
title: CircleCI Workflow
---
