---
description: Response returned when an inspection operation is successfully initiated. Contains the UUID for tracking the inspection.
layout: schema
name: InspectionResponse
properties_list:
- description: Unique identifier for the inspection operation. Use this UUID to retrieve inspection results.
  name: uuid
  type: string
- description: URL endpoint for retrieving the inspection details and results.
  name: url
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-response-schema.json
slug: deployment-rest-inspection-response
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionResponse
---
