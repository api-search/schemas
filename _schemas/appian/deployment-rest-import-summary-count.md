---
description: Summary count of items in an import deployment, showing total, imported, failed, and skipped counts.
layout: schema
name: ImportSummaryCount
properties_list:
- description: Total number of items in the package.
  name: total
  type: integer
- description: Number of items successfully imported.
  name: imported
  type: integer
- description: Number of items that failed to import.
  name: failed
  type: integer
- description: Number of items skipped during import.
  name: skipped
  type: integer
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-import-summary-count-schema.json
slug: deployment-rest-import-summary-count
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: ImportSummaryCount
---
