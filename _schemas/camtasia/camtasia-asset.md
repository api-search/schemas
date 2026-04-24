---
description: Represents a media asset in the Camtasia asset library, including video clips, audio tracks, images, animations, effects, transitions, annotations, cursors, and themes.
layout: schema
name: Camtasia Asset
properties_list:
- description: Unique identifier for the asset
  name: id
  type: string
- description: Display name of the asset
  name: name
  type: string
- description: Description of the asset
  name: description
  type: string
- description: Type of media asset
  name: type
  type: string
- description: File format (e.g., mp4, mp3, png, gif)
  name: format
  type: string
- description: File size in bytes
  name: fileSize
  type: integer
- description: Duration in seconds (for video and audio assets)
  name: duration
  type: number
- description: Width in pixels (for visual assets)
  name: width
  type: integer
- description: Height in pixels (for visual assets)
  name: height
  type: integer
- description: URL to the asset thumbnail image
  name: thumbnailUrl
  type: string
- description: URL to download the asset file
  name: downloadUrl
  type: string
- description: Tags associated with the asset
  name: tags
  type: array
- description: ID of the library containing the asset
  name: libraryId
  type: string
- description: ID of the category this asset belongs to
  name: categoryId
  type: string
- description: When the asset was created
  name: createdAt
  type: string
- description: When the asset was last modified
  name: updatedAt
  type: string
provider_name: Camtasia
provider_slug: camtasia
schema_file: json-schema/camtasia-asset-schema.json
slug: camtasia-asset
tags:
- Screen Recording
- Video Editing
- Tutorial Creation
- E-Learning
- Screencast
- oEmbed
- SDK
title: Camtasia Asset
---
