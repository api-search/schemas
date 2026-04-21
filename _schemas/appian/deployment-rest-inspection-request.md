---
description: Request body for creating a package inspection operation. Requires the deployment package and Admin Console settings files, with an optional import customization file.
layout: schema
name: InspectionRequest
properties_list:
- description: JSON string containing the inspection configuration with file name references for the attached files.
  name: json
  type: string
- description: Admin Console settings ZIP file to use for the inspection.
  name: adminConsoleSettingsFileName
  type: string
- description: The deployment package ZIP file to inspect.
  name: packageFileName
  type: string
- description: Optional import customization properties file to include in the inspection.
  name: customizationFileName
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-request-schema.json
slug: deployment-rest-inspection-request
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionRequest
---
