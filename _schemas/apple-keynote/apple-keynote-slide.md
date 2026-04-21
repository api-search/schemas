---
description: A single slide within an Apple Keynote presentation
layout: schema
name: Slide
properties_list:
- description: The 1-based position of the slide
  name: slideNumber
  type: integer
- description: The title displayed on the slide
  name: title
  type: string
- description: The slide layout name
  name: layout
  type: string
- description: Whether this slide is skipped during playback
  name: skipped
  type: boolean
- description: Presenter notes for the slide
  name: notes
  type: string
- description: Slide background color in hex
  name: backgroundColor
  type: string
provider_name: Apple Keynote
provider_slug: apple-keynote
schema_file: json-schema/apple-keynote-slide-schema.json
slug: apple-keynote-slide
tags:
- Apple
- Design
- iWork
- Presentations
- Productivity
- Slides
title: Slide
---
