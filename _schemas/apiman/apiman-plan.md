---
description: Schema representing an API plan in Apiman with associated policies
layout: schema
name: Apiman Plan
properties_list:
- description: Organization identifier owning this plan
  name: organizationId
  type: string
- description: Unique identifier for the plan
  name: id
  type: string
- description: Name of the plan
  name: name
  type: string
- description: Description of the plan
  name: description
  type: string
- description: Username of the user who created the plan
  name: createdBy
  type: string
- description: Timestamp when the plan was created
  name: createdOn
  type: string
- description: Policies applied to this plan
  name: policies
  type: array
provider_name: Apiman
provider_slug: apiman
schema_file: json-schema/apiman-plan-schema.json
slug: apiman-plan
tags:
- API Gateway
- API Management
- Developer Portal
- Java
- Open Source
title: Apiman Plan
---
