---
description: Schema representing the structure of an Apple Keynote presentation, including slides, text elements, images, shapes, transitions, and build animations.
layout: schema
name: Apple Keynote Presentation
properties_list:
- description: The title of the Keynote presentation.
  name: title
  type: string
- description: A description or subtitle for the presentation.
  name: description
  type: string
- description: The author or creator of the presentation.
  name: author
  type: string
- description: The date and time the presentation was created.
  name: createdDate
  type: string
- description: The date and time the presentation was last modified.
  name: modifiedDate
  type: string
- description: The theme applied to the presentation.
  name: theme
  type: object
- description: The dimensions of the presentation slides.
  name: slideSize
  type: object
- description: The ordered collection of slides in the presentation.
  name: slides
  type: array
- description: Additional metadata about the presentation.
  name: metadata
  type: object
provider_name: Apple Keynote
provider_slug: apple-keynote
schema_file: json-schema/apple-keynote-presentation-schema.json
slug: apple-keynote-presentation
tags:
- Apple
- Design
- iWork
- Presentations
- Productivity
- Slides
title: Apple Keynote Presentation
---
