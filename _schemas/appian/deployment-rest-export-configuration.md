---
description: Configuration for an export deployment operation specifying what to export and how.
layout: schema
name: ExportConfiguration
properties_list:
- description: Specifies the kind of export being performed. Use package for a single package or application for one or more applications.
  name: exportType
  type: string
- description: Array of UUIDs to export. For packages, provide a single UUID. For applications, provide one or more application UUIDs.
  name: uuids
  type: array
- description: Custom name for the deployment. If omitted, a name is auto-generated.
  name: name
  type: string
- description: Description of the deployment, displayed in Appian Designer.
  name: description
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-export-configuration-schema.json
slug: deployment-rest-export-configuration
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: ExportConfiguration
---
