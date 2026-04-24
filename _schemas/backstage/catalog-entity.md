---
description: A Backstage catalog entity.
layout: schema
name: Entity
properties_list:
- description: The API version of the entity schema.
  name: apiVersion
  type: string
- description: The kind of entity. Common kinds include Component, API, System, Domain, Resource, Group, User, Location, and Template.
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: The specification of the entity. The schema varies depending on the kind and type.
  name: spec
  type: object
- description: ''
  name: relations
  type: array
- description: ''
  name: status
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/catalog-entity-schema.json
slug: catalog-entity
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: Entity
---
