---
description: Collection of errors and warnings identified during a package inspection.
layout: schema
name: InspectionProblems
properties_list:
- description: Total number of errors found during inspection.
  name: totalErrors
  type: integer
- description: Total number of warnings found during inspection.
  name: totalWarnings
  type: integer
- description: Array of error details identified during inspection.
  name: errors
  type: array
- description: Array of warning details identified during inspection.
  name: warnings
  type: array
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-problems-schema.json
slug: deployment-rest-inspection-problems
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionProblems
---
