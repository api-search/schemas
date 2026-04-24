---
description: A catalog entity in Backstage representing a software component, API, resource, system, domain, group, user, location, or template within the software catalog.
layout: schema
name: Backstage Catalog Entity
properties_list:
- description: The version of the entity schema. Typically 'backstage.io/v1alpha1' or 'backstage.io/v1beta1'.
  name: apiVersion
  type: string
- description: The high-level type of the entity.
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: The specification data describing the entity, specific to its kind.
  name: spec
  type: object
- description: Relations to other entities, typically populated by the catalog processors.
  name: relations
  type: array
- description: ''
  name: status
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/backstage-entity-schema.json
slug: backstage-entity
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: Backstage Catalog Entity
---
