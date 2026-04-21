---
description: OrganizationUnit schema from Aramark Marko API
layout: schema
name: OrganizationUnit
properties_list:
- description: Unique organization unit identifier
  name: id
  type: string
- description: Organization unit name
  name: name
  type: string
- description: Organization unit type
  name: type
  type: string
- description: Parent organization unit identifier
  name: parentId
  type: string
- description: Number of locations under this unit
  name: locationCount
  type: integer
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-organization-unit-schema.json
slug: marko-api-organization-unit
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: OrganizationUnit
---
