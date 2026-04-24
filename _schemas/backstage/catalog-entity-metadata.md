---
description: Metadata common to all entity kinds.
layout: schema
name: EntityMetadata
properties_list:
- description: A globally unique identifier for the entity.
  name: uid
  type: string
- description: An opaque string that changes on each update.
  name: etag
  type: string
- description: The name of the entity.
  name: name
  type: string
- description: The namespace the entity belongs to.
  name: namespace
  type: string
- description: A human-readable title for the entity.
  name: title
  type: string
- description: A human-readable description of the entity.
  name: description
  type: string
- description: Key-value pairs for labeling the entity.
  name: labels
  type: object
- description: Key-value pairs for non-identifying metadata.
  name: annotations
  type: object
- description: A list of single-valued strings for classification.
  name: tags
  type: array
- description: ''
  name: links
  type: array
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/catalog-entity-metadata-schema.json
slug: catalog-entity-metadata
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: EntityMetadata
---
