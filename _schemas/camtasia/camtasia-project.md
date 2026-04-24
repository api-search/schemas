---
description: Represents a Camtasia video editing project, including canvas settings, timeline configuration, and production metadata.
layout: schema
name: Camtasia Project
properties_list:
- description: Unique identifier for the project
  name: id
  type: string
- description: Project name
  name: name
  type: string
- description: Project description
  name: description
  type: string
- description: Current project status
  name: status
  type: string
- description: Project canvas resolution
  name: resolution
  type: object
- description: Project frame rate in frames per second
  name: frameRate
  type: number
- description: Total project duration in seconds
  name: duration
  type: number
- description: Number of timeline tracks
  name: trackCount
  type: integer
- description: ID of the template used to create this project
  name: templateId
  type: string
- description: When the project was created
  name: createdAt
  type: string
- description: When the project was last modified
  name: updatedAt
  type: string
provider_name: Camtasia
provider_slug: camtasia
schema_file: json-schema/camtasia-project-schema.json
slug: camtasia-project
tags:
- Screen Recording
- Video Editing
- Tutorial Creation
- E-Learning
- Screencast
- oEmbed
- SDK
title: Camtasia Project
---
