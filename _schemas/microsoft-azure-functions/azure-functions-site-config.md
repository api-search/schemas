---
description: Configuration of an App Service app.
layout: schema
name: SiteConfig
properties_list:
- description: Number of workers.
  name: numberOfWorkers
  type: integer
- description: Default documents.
  name: defaultDocuments
  type: array
- description: .NET Framework version.
  name: netFrameworkVersion
  type: string
- description: Version of PHP.
  name: phpVersion
  type: string
- description: Version of Python.
  name: pythonVersion
  type: string
- description: Version of Node.js.
  name: nodeVersion
  type: string
- description: Version of PowerShell.
  name: powerShellVersion
  type: string
- description: Linux App Framework and version
  name: linuxFxVersion
  type: string
- description: Xenon App Framework and version
  name: windowsFxVersion
  type: string
- description: <code>true</code> if request tracing is enabled; otherwise, <code>false</code>.
  name: requestTracingEnabled
  type: boolean
- description: Request tracing expiration time.
  name: requestTracingExpirationTime
  type: string
- description: <code>true</code> if remote debugging is enabled; otherwise, <code>false</code>.
  name: remoteDebuggingEnabled
  type: boolean
- description: Remote debugging version.
  name: remoteDebuggingVersion
  type: string
- description: <code>true</code> if HTTP logging is enabled; otherwise, <code>false</code>.
  name: httpLoggingEnabled
  type: boolean
- description: Flag to use Managed Identity Creds for ACR pull
  name: acrUseManagedIdentityCreds
  type: boolean
- description: If using user managed identity, the user managed identity ClientId
  name: acrUserManagedIdentityID
  type: string
- description: HTTP logs directory size limit.
  name: logsDirectorySizeLimit
  type: integer
- description: <code>true</code> if detailed error logging is enabled; otherwise, <code>false</code>.
  name: detailedErrorLoggingEnabled
  type: boolean
- description: Publishing user name.
  name: publishingUsername
  type: string
- description: Application settings. This property is not returned in response to normal create and read requests since it may contain sensitive information.
  name: appSettings
  type: array
- description: Application metadata. This property cannot be retrieved, since it may contain secrets.
  name: metadata
  type: array
- description: Connection strings. This property is not returned in response to normal create and read requests since it may contain sensitive information.
  name: connectionStrings
  type: array
- description: Site MachineKey.
  name: machineKey
  type: object
- description: Handler mappings.
  name: handlerMappings
  type: array
- description: Document root.
  name: documentRoot
  type: string
- description: SCM type.
  name: scmType
  type: object
- description: <code>true</code> to use 32-bit worker process; otherwise, <code>false</code>.
  name: use32BitWorkerProcess
  type: boolean
- description: <code>true</code> if WebSocket is enabled; otherwise, <code>false</code>.
  name: webSocketsEnabled
  type: boolean
- description: <code>true</code> if Always On is enabled; otherwise, <code>false</code>.
  name: alwaysOn
  type: boolean
- description: Java version.
  name: javaVersion
  type: string
- description: Java container.
  name: javaContainer
  type: string
- description: Java container version.
  name: javaContainerVersion
  type: string
- description: App command line to launch.
  name: appCommandLine
  type: string
- description: Managed pipeline mode.
  name: managedPipelineMode
  type: object
- description: Virtual applications.
  name: virtualApplications
  type: array
- description: Site load balancing.
  name: loadBalancing
  type: object
- description: This is work around for polymorphic types.
  name: experiments
  type: object
- description: Site limits.
  name: limits
  type: object
- description: <code>true</code> if Auto Heal is enabled; otherwise, <code>false</code>.
  name: autoHealEnabled
  type: boolean
- description: Auto Heal rules.
  name: autoHealRules
  type: object
- description: Tracing options.
  name: tracingOptions
  type: string
- description: Virtual Network name.
  name: vnetName
  type: string
- description: Virtual Network Route All enabled. This causes all outbound traffic to have Virtual Network Security Groups and User Defined Routes applied.
  name: vnetRouteAllEnabled
  type: boolean
- description: The number of private ports assigned to this app. These will be assigned dynamically on runtime.
  name: vnetPrivatePortsCount
  type: integer
- description: Cross-Origin Resource Sharing (CORS) settings.
  name: cors
  type: object
- description: Push endpoint settings.
  name: push
  type: object
- description: Information about the formal API definition for the app.
  name: apiDefinition
  type: object
- description: Azure API management settings linked to the app.
  name: apiManagementConfig
  type: object
- description: Auto-swap slot name.
  name: autoSwapSlotName
  type: string
- description: <code>true</code> to enable local MySQL; otherwise, <code>false</code>.
  name: localMySqlEnabled
  type: boolean
- description: Managed Service Identity Id
  name: managedServiceIdentityId
  type: integer
- description: Explicit Managed Service Identity Id
  name: xManagedServiceIdentityId
  type: integer
- description: Identity to use for Key Vault Reference authentication.
  name: keyVaultReferenceIdentity
  type: string
- description: IP security restrictions for main.
  name: ipSecurityRestrictions
  type: array
- description: Default action for main access restriction if no rules are matched.
  name: ipSecurityRestrictionsDefaultAction
  type: object
- description: IP security restrictions for scm.
  name: scmIpSecurityRestrictions
  type: array
- description: Default action for scm access restriction if no rules are matched.
  name: scmIpSecurityRestrictionsDefaultAction
  type: object
- description: IP security restrictions for scm to use main.
  name: scmIpSecurityRestrictionsUseMain
  type: boolean
- description: 'Http20Enabled: configures a web site to allow clients to connect over http2.0'
  name: http20Enabled
  type: boolean
- description: 'Http20ProxyFlag: Configures a website to allow http2.0 to pass be proxied all the way to the app. 0 = disabled, 1 = pass through all http2 traffic, 2 = pass through gRPC only.'
  name: http20ProxyFlag
  type: integer
- description: 'MinTlsVersion: configures the minimum version of TLS required for SSL requests'
  name: minTlsVersion
  type: object
- description: The minimum strength TLS cipher suite allowed for an application
  name: minTlsCipherSuite
  type: object
- description: 'ScmMinTlsVersion: configures the minimum version of TLS required for SSL requests for SCM site'
  name: scmMinTlsVersion
  type: object
- description: State of FTP / FTPS service
  name: ftpsState
  type: object
- description: Number of preWarmed instances. This setting only applies to the Consumption and Elastic Plans
  name: preWarmedInstanceCount
  type: integer
- description: Maximum number of workers that a site can scale out to. This setting only applies to the Consumption and Elastic Premium Plans
  name: functionAppScaleLimit
  type: integer
- description: Maximum number of workers that a site can scale out to. This setting only applies to apps in plans where ElasticScaleEnabled is <code>true</code>
  name: elasticWebAppScaleLimit
  type: integer
- description: Health check path
  name: healthCheckPath
  type: string
- description: Gets or sets a value indicating whether functions runtime scale monitoring is enabled. When enabled, the ScaleController will not monitor event sources directly, but will instead call to the runtime t
  name: functionsRuntimeScaleMonitoringEnabled
  type: boolean
- description: Sets the time zone a site uses for generating timestamps. Compatible with Linux and Windows App Service. Setting the WEBSITE_TIME_ZONE app setting takes precedence over this config. For Linux, expects
  name: websiteTimeZone
  type: string
- description: Number of minimum instance count for a site This setting only applies to the Elastic Plans
  name: minimumElasticInstanceCount
  type: integer
- description: List of Azure Storage Accounts.
  name: azureStorageAccounts
  type: object
- description: Property to allow or block all public traffic.
  name: publicNetworkAccess
  type: string
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-site-config-schema.json
slug: azure-functions-site-config
source_filename: azure-functions-site-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-site-config-schema.json\",\n  \"title\": \"SiteConfig\",\n  \"description\": \"Configuration of an App Service app.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"numberOfWorkers\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of workers.\"\n    },\n    \"defaultDocuments\": {\n      \"type\": \"array\",\n      \"description\": \"Default documents.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"netFrameworkVersion\": {\n      \"type\": \"string\",\n      \"description\": \".NET Framework version.\",\n      \"default\": \"v4.6\"\n    },\n    \"phpVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of PHP.\"\n    },\n    \"pythonVersion\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Version of Python.\"\n    },\n    \"nodeVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of Node.js.\"\n    },\n    \"powerShellVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of PowerShell.\"\n    },\n    \"linuxFxVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Linux App Framework and version\"\n    },\n    \"windowsFxVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Xenon App Framework and version\"\n    },\n    \"requestTracingEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"<code>true</code> if request tracing is enabled; otherwise, <code>false</code>.\"\n    },\n    \"requestTracingExpirationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Request tracing expiration time.\"\n    },\n    \"remoteDebuggingEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"<code>true</code> if remote\
  \ debugging is enabled; otherwise, <code>false</code>.\"\n    },\n    \"remoteDebuggingVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Remote debugging version.\"\n    },\n    \"httpLoggingEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"<code>true</code> if HTTP logging is enabled; otherwise, <code>false</code>.\"\n    },\n    \"acrUseManagedIdentityCreds\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag to use Managed Identity Creds for ACR pull\"\n    },\n    \"acrUserManagedIdentityID\": {\n      \"type\": \"string\",\n      \"description\": \"If using user managed identity, the user managed identity ClientId\"\n    },\n    \"logsDirectorySizeLimit\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"HTTP logs directory size limit.\"\n    },\n    \"detailedErrorLoggingEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"<code>true</code> if detailed error logging is enabled;\
  \ otherwise, <code>false</code>.\"\n    },\n    \"publishingUsername\": {\n      \"type\": \"string\",\n      \"description\": \"Publishing user name.\"\n    },\n    \"appSettings\": {\n      \"type\": \"array\",\n      \"description\": \"Application settings. This property is not returned in response to normal create and read requests since it may contain sensitive information.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/NameValuePair\"\n      },\n      \"x-ms-identifiers\": [\n        \"name\"\n      ],\n      \"x-ms-mutability\": [\n        \"update\",\n        \"create\"\n      ]\n    },\n    \"metadata\": {\n      \"type\": \"array\",\n      \"description\": \"Application metadata. This property cannot be retrieved, since it may contain secrets.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/NameValuePair\"\n      },\n      \"x-ms-identifiers\": [\n        \"name\"\n      ],\n      \"x-ms-mutability\": [\n        \"update\",\n        \"create\"\n      ]\n\
  \    },\n    \"connectionStrings\": {\n      \"type\": \"array\",\n      \"description\": \"Connection strings. This property is not returned in response to normal create and read requests since it may contain sensitive information.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ConnStringInfo\"\n      },\n      \"x-ms-identifiers\": [\n        \"name\"\n      ],\n      \"x-ms-mutability\": [\n        \"update\",\n        \"create\"\n      ]\n    },\n    \"machineKey\": {\n      \"$ref\": \"#/definitions/SiteMachineKey\",\n      \"description\": \"Site MachineKey.\",\n      \"readOnly\": true\n    },\n    \"handlerMappings\": {\n      \"type\": \"array\",\n      \"description\": \"Handler mappings.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/HandlerMapping\"\n      },\n      \"x-ms-identifiers\": [\n        \"extension\"\n      ]\n    },\n    \"documentRoot\": {\n      \"type\": \"string\",\n      \"description\": \"Document root.\"\n    },\n    \"scmType\": {\n\
  \      \"$ref\": \"#/definitions/ScmType\",\n      \"description\": \"SCM type.\"\n    },\n    \"use32BitWorkerProcess\": {\n      \"type\": \"boolean\",\n      \"description\": \"<code>true</code> to use 32-bit worker process; otherwise, <code>false</code>.\"\n    },\n    \"webSocketsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"<code>true</code> if WebSocket is enabled; otherwise, <code>false</code>.\"\n    },\n    \"alwaysOn\": {\n      \"type\": \"boolean\",\n      \"description\": \"<code>true</code> if Always On is enabled; otherwise, <code>false</code>.\"\n    },\n    \"javaVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Java version.\"\n    },\n    \"javaContainer\": {\n      \"type\": \"string\",\n      \"description\": \"Java container.\"\n    },\n    \"javaContainerVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Java container version.\"\n    },\n    \"appCommandLine\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"App command line to launch.\"\n    },\n    \"managedPipelineMode\": {\n      \"$ref\": \"#/definitions/ManagedPipelineMode\",\n      \"description\": \"Managed pipeline mode.\"\n    },\n    \"virtualApplications\": {\n      \"type\": \"array\",\n      \"description\": \"Virtual applications.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/VirtualApplication\"\n      },\n      \"x-ms-identifiers\": [\n        \"virtualPath\"\n      ]\n    },\n    \"loadBalancing\": {\n      \"$ref\": \"#/definitions/SiteLoadBalancing\",\n      \"description\": \"Site load balancing.\"\n    },\n    \"experiments\": {\n      \"$ref\": \"#/definitions/Experiments\",\n      \"description\": \"This is work around for polymorphic types.\"\n    },\n    \"limits\": {\n      \"$ref\": \"#/definitions/SiteLimits\",\n      \"description\": \"Site limits.\"\n    },\n    \"autoHealEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"<code>true</code> if Auto Heal is enabled; otherwise,\
  \ <code>false</code>.\"\n    },\n    \"autoHealRules\": {\n      \"$ref\": \"#/definitions/AutoHealRules\",\n      \"description\": \"Auto Heal rules.\"\n    },\n    \"tracingOptions\": {\n      \"type\": \"string\",\n      \"description\": \"Tracing options.\"\n    },\n    \"vnetName\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual Network name.\",\n      \"x-ms-mutability\": [\n        \"read\",\n        \"create\"\n      ]\n    },\n    \"vnetRouteAllEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Virtual Network Route All enabled. This causes all outbound traffic to have Virtual Network Security Groups and User Defined Routes applied.\"\n    },\n    \"vnetPrivatePortsCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"The number of private ports assigned to this app. These will be assigned dynamically on runtime.\"\n    },\n    \"cors\": {\n      \"$ref\": \"#/definitions/CorsSettings\",\n      \"description\"\
  : \"Cross-Origin Resource Sharing (CORS) settings.\"\n    },\n    \"push\": {\n      \"$ref\": \"#/definitions/PushSettings\",\n      \"description\": \"Push endpoint settings.\"\n    },\n    \"apiDefinition\": {\n      \"$ref\": \"#/definitions/ApiDefinitionInfo\",\n      \"description\": \"Information about the formal API definition for the app.\"\n    },\n    \"apiManagementConfig\": {\n      \"$ref\": \"#/definitions/ApiManagementConfig\",\n      \"description\": \"Azure API management settings linked to the app.\"\n    },\n    \"autoSwapSlotName\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-swap slot name.\"\n    },\n    \"localMySqlEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"<code>true</code> to enable local MySQL; otherwise, <code>false</code>.\",\n      \"default\": false\n    },\n    \"managedServiceIdentityId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Managed Service Identity Id\"\n  \
  \  },\n    \"xManagedServiceIdentityId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Explicit Managed Service Identity Id\"\n    },\n    \"keyVaultReferenceIdentity\": {\n      \"type\": \"string\",\n      \"description\": \"Identity to use for Key Vault Reference authentication.\"\n    },\n    \"ipSecurityRestrictions\": {\n      \"type\": \"array\",\n      \"description\": \"IP security restrictions for main.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/IpSecurityRestriction\"\n      },\n      \"x-ms-identifiers\": [\n        \"name\"\n      ]\n    },\n    \"ipSecurityRestrictionsDefaultAction\": {\n      \"$ref\": \"#/definitions/DefaultAction\",\n      \"description\": \"Default action for main access restriction if no rules are matched.\"\n    },\n    \"scmIpSecurityRestrictions\": {\n      \"type\": \"array\",\n      \"description\": \"IP security restrictions for scm.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/IpSecurityRestriction\"\
  \n      },\n      \"x-ms-identifiers\": [\n        \"name\"\n      ]\n    },\n    \"scmIpSecurityRestrictionsDefaultAction\": {\n      \"$ref\": \"#/definitions/DefaultAction\",\n      \"description\": \"Default action for scm access restriction if no rules are matched.\"\n    },\n    \"scmIpSecurityRestrictionsUseMain\": {\n      \"type\": \"boolean\",\n      \"description\": \"IP security restrictions for scm to use main.\"\n    },\n    \"http20Enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Http20Enabled: configures a web site to allow clients to connect over http2.0\",\n      \"default\": true\n    },\n    \"http20ProxyFlag\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Http20ProxyFlag: Configures a website to allow http2.0 to pass be proxied all the way to the app. 0 = disabled, 1 = pass through all http2 traffic, 2 = pass through gRPC only.\",\n      \"default\": 0\n    },\n    \"minTlsVersion\": {\n      \"$ref\":\
  \ \"#/definitions/SupportedTlsVersions\",\n      \"description\": \"MinTlsVersion: configures the minimum version of TLS required for SSL requests\"\n    },\n    \"minTlsCipherSuite\": {\n      \"$ref\": \"#/definitions/TlsCipherSuites\",\n      \"description\": \"The minimum strength TLS cipher suite allowed for an application\"\n    },\n    \"scmMinTlsVersion\": {\n      \"$ref\": \"#/definitions/SupportedTlsVersions\",\n      \"description\": \"ScmMinTlsVersion: configures the minimum version of TLS required for SSL requests for SCM site\"\n    },\n    \"ftpsState\": {\n      \"$ref\": \"#/definitions/FtpsState\",\n      \"description\": \"State of FTP / FTPS service\"\n    },\n    \"preWarmedInstanceCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of preWarmed instances.\\nThis setting only applies to the Consumption and Elastic Plans\",\n      \"minimum\": 0,\n      \"maximum\": 10\n    },\n    \"functionAppScaleLimit\": {\n \
  \     \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Maximum number of workers that a site can scale out to.\\nThis setting only applies to the Consumption and Elastic Premium Plans\",\n      \"minimum\": 0\n    },\n    \"elasticWebAppScaleLimit\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Maximum number of workers that a site can scale out to.\\nThis setting only applies to apps in plans where ElasticScaleEnabled is <code>true</code>\",\n      \"minimum\": 0\n    },\n    \"healthCheckPath\": {\n      \"type\": \"string\",\n      \"description\": \"Health check path\"\n    },\n    \"functionsRuntimeScaleMonitoringEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Gets or sets a value indicating whether functions runtime scale monitoring is enabled. When enabled,\\nthe ScaleController will not monitor event sources directly, but will instead call to the\\nruntime to get scale status.\"\n    },\n\
  \    \"websiteTimeZone\": {\n      \"type\": \"string\",\n      \"description\": \"Sets the time zone a site uses for generating timestamps. Compatible with Linux and Windows App Service. Setting the WEBSITE_TIME_ZONE app setting takes precedence over this config. For Linux, expects tz database values https://www.iana.org/time-zones (for a quick reference see https://en.wikipedia.org/wiki/List_of_tz_database_time_zones). For Windows, expects one of the time zones listed under HKEY_LOCAL_MACHINE\\\\SOFTWARE\\\\Microsoft\\\\Windows NT\\\\CurrentVersion\\\\Time Zones\"\n    },\n    \"minimumElasticInstanceCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of minimum instance count for a site\\nThis setting only applies to the Elastic Plans\",\n      \"minimum\": 0,\n      \"maximum\": 20\n    },\n    \"azureStorageAccounts\": {\n      \"type\": \"object\",\n      \"description\": \"List of Azure Storage Accounts.\",\n      \"additionalProperties\"\
  : {\n        \"$ref\": \"#/definitions/AzureStorageInfoValue\"\n      }\n    },\n    \"publicNetworkAccess\": {\n      \"type\": \"string\",\n      \"description\": \"Property to allow or block all public traffic.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-site-config-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: SiteConfig
---
