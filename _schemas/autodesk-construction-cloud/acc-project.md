---
description: JSON Schema for an Autodesk Construction Cloud (ACC) project.
layout: schema
name: Autodesk Construction Cloud Project
properties_list:
- description: Unique ACC project identifier
  name: id
  type: string
- description: Parent account identifier
  name: accountId
  type: string
- description: Project name
  name: name
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: projectValue
  type: object
- description: ''
  name: status
  type: string
- description: ''
  name: jobNumber
  type: string
- description: ''
  name: addressLine1
  type: string
- description: ''
  name: addressLine2
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: stateOrProvince
  type: string
- description: ''
  name: postalCode
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: timezone
  type: string
- description: ''
  name: language
  type: string
- description: Type of construction (e.g., New Construction, Renovation, Infrastructure)
  name: constructionType
  type: string
- description: Project delivery method (e.g., Design-Build, Design-Bid-Build, CM at Risk)
  name: deliveryMethod
  type: string
- description: Contract type (e.g., Fixed Price, Cost Plus, Unit Price)
  name: contractType
  type: string
- description: Current project phase
  name: currentPhase
  type: string
- description: ''
  name: businessUnitsId
  type: string
- description: ''
  name: imageUrl
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Autodesk Construction Cloud
provider_slug: autodesk-construction-cloud
schema_file: json-schema/acc-project-schema.json
slug: acc-project
tags:
- Construction
- BIM
- Project Management
- AEC
- CAD
- Architecture
- Engineering
- Field Management
title: Autodesk Construction Cloud Project
---
