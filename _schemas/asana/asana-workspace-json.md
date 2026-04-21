---
description: A workspace is the highest-level organizational unit in Asana. All projects and tasks have an associated workspace. An organization is a special kind of workspace that represents a company.
layout: schema
name: Asana Workspace
properties_list:
- description: Globally unique identifier of the resource.
  name: gid
  type: string
- description: The base type of this resource.
  name: resource_type
  type: string
- description: The name of the workspace.
  name: name
  type: string
- description: Whether the workspace is an organization.
  name: is_organization
  type: boolean
- description: The email domains associated with this workspace.
  name: email_domains
  type: array
provider_name: Asana
provider_slug: asana
schema_file: json-schema/asana-workspace-json-schema.json
slug: asana-workspace-json
tags:
- Collaboration
- Productivity
- Project Management
- Projects
- Task Management
- Tasks
- Workflow
title: Asana Workspace
---
