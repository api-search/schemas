---
description: A Banuba augmented reality effect that can be applied to a face in a video frame.
layout: schema
name: AREffect
properties_list:
- description: Unique identifier for the AR effect.
  name: effectId
  type: string
- description: Human-readable name of the effect.
  name: name
  type: string
- description: Category of the effect.
  name: category
  type: string
- description: URL of a preview image for the effect.
  name: previewUrl
  type: string
- description: URL of the effect bundle file.
  name: effectUrl
  type: string
- description: Platforms supported by this effect.
  name: platforms
  type: array
- description: Tags describing the effect.
  name: tags
  type: array
provider_name: Banuba
provider_slug: banuba
schema_file: json-schema/areffect-schema.json
slug: areffect
tags:
- AR
- Augmented Reality
- Beauty
- Face Recognition
- Facial
- SDK
- Video
title: AREffect
---
