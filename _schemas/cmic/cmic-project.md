---
description: Schema representing a construction project in the CMiC ERP system.
layout: schema
name: CMiC Construction Project
properties_list:
- description: Unique project identifier in CMiC
  name: projectId
  type: string
- description: Project name
  name: projectName
  type: string
- description: CMiC company code for multi-company setups
  name: companyCode
  type: string
- description: Project description
  name: description
  type: string
- description: Project status
  name: status
  type: string
- description: Project manager name or employee ID
  name: projectManager
  type: string
- description: Project owner organization name
  name: owner
  type: string
- description: Project start date
  name: startDate
  type: string
- description: Project completion date
  name: endDate
  type: string
- description: Project site address
  name: address
  type: object
- description: Project financial summary
  name: financials
  type: object
- description: List of job IDs associated with this project
  name: jobs
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: CMiC
provider_slug: cmic
schema_file: json-schema/cmic-project-schema.json
slug: cmic-project
tags:
- Construction
- ERP
- Finance
- Project Management
title: CMiC Construction Project
---
