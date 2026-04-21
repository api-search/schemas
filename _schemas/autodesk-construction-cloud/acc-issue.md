---
description: JSON Schema for an ACC construction issue, observation, or punch list item.
layout: schema
name: Autodesk Construction Cloud Issue
properties_list:
- description: Unique issue identifier (UUID)
  name: id
  type: string
- description: ACC project container identifier
  name: containerId
  type: string
- description: Human-readable sequential issue number
  name: displayId
  type: integer
- description: Issue title/summary
  name: title
  type: string
- description: Detailed issue description
  name: description
  type: string
- description: Current issue status
  name: status
  type: string
- description: Issue type identifier
  name: issueTypeId
  type: string
- description: Issue subtype identifier
  name: issueSubtypeId
  type: string
- description: ''
  name: dueDate
  type: string
- description: ''
  name: startDate
  type: string
- description: Location identifier within the project
  name: locationId
  type: string
- description: Free-text location description
  name: locationDescription
  type: string
- description: User or company assigned to resolve the issue
  name: assignedToId
  type: string
- description: ''
  name: assignedToType
  type: string
- description: User ID who created the issue
  name: createdBy
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: ''
  name: closedBy
  type: string
- description: ''
  name: closedAt
  type: string
- description: ''
  name: rootCauseId
  type: string
- description: ''
  name: commentCount
  type: integer
- description: ''
  name: attachmentCount
  type: integer
- description: ''
  name: linkedDocuments
  type: array
provider_name: Autodesk Construction Cloud
provider_slug: autodesk-construction-cloud
schema_file: json-schema/acc-issue-schema.json
slug: acc-issue
tags:
- Construction
- BIM
- Project Management
- AEC
- CAD
- Architecture
- Engineering
- Field Management
title: Autodesk Construction Cloud Issue
---
