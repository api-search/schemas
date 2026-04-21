---
description: A warning identified during package inspection that may affect deployment but would not prevent it.
layout: schema
name: InspectionWarning
properties_list:
- description: A description of the warning condition.
  name: warningMessage
  type: string
- description: The name of the object associated with the warning.
  name: objectName
  type: string
- description: The UUID of the object associated with the warning.
  name: objectUuid
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-warning-schema.json
slug: deployment-rest-inspection-warning
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionWarning
---
