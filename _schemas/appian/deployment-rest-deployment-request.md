---
description: Request body for creating a deployment operation. For exports, provide the JSON configuration with export type and UUIDs. For imports, provide package files along with the JSON configuration.
layout: schema
name: DeploymentRequest
properties_list:
- description: JSON string containing the deployment configuration. For exports, includes exportType and uuids. For imports, includes name, description, and file name references.
  name: json
  type: string
- description: The deployment package ZIP file to import. Required for import operations.
  name: packageFileName
  type: string
- description: Admin Console settings ZIP file to import alongside the package.
  name: adminConsoleSettingsFileName
  type: string
- description: Import customization properties file that maps source environment values to target environment values.
  name: customizationFileName
  type: string
- description: Plug-ins ZIP file containing plug-ins to deploy.
  name: pluginsFileName
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-deployment-request-schema.json
slug: deployment-rest-deployment-request
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: DeploymentRequest
---
