---
description: An error identified during package inspection that would prevent successful deployment.
layout: schema
name: InspectionError
properties_list:
- description: A description of the error condition.
  name: errorMessage
  type: string
- description: The name of the object affected by the error.
  name: objectName
  type: string
- description: The UUID of the object affected by the error.
  name: objectUuid
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-error-schema.json
slug: deployment-rest-inspection-error
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionError
---
