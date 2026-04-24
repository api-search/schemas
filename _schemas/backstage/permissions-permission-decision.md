---
description: PermissionDecision schema from Backstage permissions API
layout: schema
name: PermissionDecision
properties_list:
- description: The authorization decision result.
  name: result
  type: string
- description: The plugin responsible for condition evaluation.
  name: pluginId
  type: string
- description: The resource type for conditional decisions.
  name: resourceType
  type: string
- description: The conditions that must be evaluated against the resource to produce a final decision. Only present when result is CONDITIONAL.
  name: conditions
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/permissions-permission-decision-schema.json
slug: permissions-permission-decision
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: PermissionDecision
---
