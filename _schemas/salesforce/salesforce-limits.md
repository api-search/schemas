---
description: ''
layout: schema
name: Limits
properties_list:
- description: ''
  name: ActiveScratchOrgs
  type: object
- description: ''
  name: AnalyticsExternalDataSizeMB
  type: object
- description: ''
  name: ConcurrentAsyncGetReportInstances
  type: object
- description: ''
  name: ConcurrentEinsteinDataInsightsStoryCreation
  type: object
- description: ''
  name: ConcurrentEinsteinDiscoveryStoryCreation
  type: object
- description: ''
  name: ConcurrentSyncReportRuns
  type: object
- description: ''
  name: DailyAnalyticsDataflowJobExecutions
  type: object
- description: ''
  name: DailyAnalyticsUploadedFilesSizeMB
  type: object
- description: ''
  name: DailyApiRequests
  type: object
- description: ''
  name: DailyAsyncApexExecutions
  type: object
- description: ''
  name: DailyAsyncApexTests
  type: object
- description: ''
  name: DailyBulkApiBatches
  type: object
- description: ''
  name: DailyBulkV2QueryFileStorageMB
  type: object
- description: ''
  name: DailyBulkV2QueryJobs
  type: object
- description: ''
  name: DailyDeliveredPlatformEvents
  type: object
- description: ''
  name: DailyDurableGenericStreamingApiEvents
  type: object
- description: ''
  name: DailyDurableStreamingApiEvents
  type: object
- description: ''
  name: DailyEinsteinDataInsightsStoryCreation
  type: object
- description: ''
  name: DailyEinsteinDiscoveryOptimizationJobRuns
  type: object
- description: ''
  name: DailyEinsteinDiscoveryPredictAPICalls
  type: object
- description: ''
  name: DailyEinsteinDiscoveryPredictionsByCDC
  type: object
- description: ''
  name: DailyEinsteinDiscoveryStoryCreation
  type: object
- description: ''
  name: DailyFunctionsApiCallLimit
  type: object
- description: ''
  name: DailyGenericStreamingApiEvents
  type: object
- description: ''
  name: DailyScratchOrgs
  type: object
- description: ''
  name: DailyStandardVolumePlatformEvents
  type: object
- description: ''
  name: DailyStreamingApiEvents
  type: object
- description: ''
  name: DailyWorkflowEmails
  type: object
- description: ''
  name: DataStorageMB
  type: object
- description: ''
  name: DurableStreamingApiConcurrentClients
  type: object
- description: ''
  name: FileStorageMB
  type: object
- description: ''
  name: HourlyAsyncReportRuns
  type: object
- description: ''
  name: HourlyDashboardRefreshes
  type: object
- description: ''
  name: HourlyDashboardResults
  type: object
- description: ''
  name: HourlyDashboardStatuses
  type: object
- description: ''
  name: HourlyLongTermIdMapping
  type: object
- description: ''
  name: HourlyManagedContentPublicRequests
  type: object
- description: ''
  name: HourlyODataCallout
  type: object
- description: ''
  name: HourlyPublishedPlatformEvents
  type: object
- description: ''
  name: HourlyPublishedStandardVolumePlatformEvents
  type: object
- description: ''
  name: HourlyShortTermIdMapping
  type: object
- description: ''
  name: HourlySyncReportRuns
  type: object
- description: ''
  name: HourlyTimeBasedWorkflow
  type: object
- description: ''
  name: MassEmail
  type: object
- description: ''
  name: MonthlyEinsteinDiscoveryStoryCreation
  type: object
- description: ''
  name: Package2VersionCreates
  type: object
- description: ''
  name: Package2VersionCreatesWithoutValidation
  type: object
- description: ''
  name: PermissionSets
  type: object
- description: ''
  name: PrivateConnectOutboundCalloutHourlyLimitMB
  type: object
- description: ''
  name: PublishCallbackUsageInApex
  type: object
- description: ''
  name: SingleEmail
  type: object
- description: ''
  name: StreamingApiConcurrentClients
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-limits-schema.json
slug: salesforce-limits
source_filename: salesforce-limits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActiveScratchOrgs\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"AnalyticsExternalDataSizeMB\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"ConcurrentAsyncGetReportInstances\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n   \
  \     \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"ConcurrentEinsteinDataInsightsStoryCreation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"ConcurrentEinsteinDiscoveryStoryCreation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"ConcurrentSyncReportRuns\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyAnalyticsDataflowJobExecutions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyAnalyticsUploadedFilesSizeMB\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\"\
  : 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyApiRequests\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyAsyncApexExecutions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyAsyncApexTests\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\"\
  : 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyBulkApiBatches\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyBulkV2QueryFileStorageMB\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyBulkV2QueryJobs\": {\n      \"type\"\
  : \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyDeliveredPlatformEvents\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyDurableGenericStreamingApiEvents\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n     \
  \ },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyDurableStreamingApiEvents\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyEinsteinDataInsightsStoryCreation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyEinsteinDiscoveryOptimizationJobRuns\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\"\
  : \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyEinsteinDiscoveryPredictAPICalls\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyEinsteinDiscoveryPredictionsByCDC\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n\
  \      ]\n    },\n    \"DailyEinsteinDiscoveryStoryCreation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyFunctionsApiCallLimit\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyGenericStreamingApiEvents\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n      \
  \    \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyScratchOrgs\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyStandardVolumePlatformEvents\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyStreamingApiEvents\": {\n      \"type\": \"object\",\n      \"properties\": {\n    \
  \    \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DailyWorkflowEmails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"DataStorageMB\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n\
  \    },\n    \"DurableStreamingApiConcurrentClients\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"FileStorageMB\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlyAsyncReportRuns\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n  \
  \        \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlyDashboardRefreshes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlyDashboardResults\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlyDashboardStatuses\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\"\
  : \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlyLongTermIdMapping\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlyManagedContentPublicRequests\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n\
  \    \"HourlyODataCallout\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlyPublishedPlatformEvents\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlyPublishedStandardVolumePlatformEvents\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\"\
  ,\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlyShortTermIdMapping\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlySyncReportRuns\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"HourlyTimeBasedWorkflow\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\"\
  : \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"MassEmail\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"MonthlyEinsteinDiscoveryStoryCreation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"Package2VersionCreates\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"Package2VersionCreatesWithoutValidation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"PermissionSets\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n\
  \        \"CreateCustom\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Max\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            },\n            \"Remaining\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            }\n          },\n          \"required\": [\n            \"Max\",\n            \"Remaining\"\n          ]\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\",\n        \"CreateCustom\"\n      ]\n    },\n    \"PrivateConnectOutboundCalloutHourlyLimitMB\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"PublishCallbackUsageInApex\": {\n      \"type\": \"object\"\
  ,\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"SingleEmail\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    },\n    \"StreamingApiConcurrentClients\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"\
  Max\",\n        \"Remaining\"\n      ]\n    }\n  },\n  \"required\": [\n    \"ActiveScratchOrgs\",\n    \"AnalyticsExternalDataSizeMB\",\n    \"ConcurrentAsyncGetReportInstances\",\n    \"ConcurrentEinsteinDataInsightsStoryCreation\",\n    \"ConcurrentEinsteinDiscoveryStoryCreation\",\n    \"ConcurrentSyncReportRuns\",\n    \"DailyAnalyticsDataflowJobExecutions\",\n    \"DailyAnalyticsUploadedFilesSizeMB\",\n    \"DailyApiRequests\",\n    \"DailyAsyncApexExecutions\",\n    \"DailyAsyncApexTests\",\n    \"DailyBulkApiBatches\",\n    \"DailyBulkV2QueryFileStorageMB\",\n    \"DailyBulkV2QueryJobs\",\n    \"DailyDeliveredPlatformEvents\",\n    \"DailyDurableGenericStreamingApiEvents\",\n    \"DailyDurableStreamingApiEvents\",\n    \"DailyEinsteinDataInsightsStoryCreation\",\n    \"DailyEinsteinDiscoveryOptimizationJobRuns\",\n    \"DailyEinsteinDiscoveryPredictAPICalls\",\n    \"DailyEinsteinDiscoveryPredictionsByCDC\",\n    \"DailyEinsteinDiscoveryStoryCreation\",\n    \"DailyFunctionsApiCallLimit\"\
  ,\n    \"DailyGenericStreamingApiEvents\",\n    \"DailyScratchOrgs\",\n    \"DailyStandardVolumePlatformEvents\",\n    \"DailyStreamingApiEvents\",\n    \"DailyWorkflowEmails\",\n    \"DataStorageMB\",\n    \"DurableStreamingApiConcurrentClients\",\n    \"FileStorageMB\",\n    \"HourlyAsyncReportRuns\",\n    \"HourlyDashboardRefreshes\",\n    \"HourlyDashboardResults\",\n    \"HourlyDashboardStatuses\",\n    \"HourlyLongTermIdMapping\",\n    \"HourlyManagedContentPublicRequests\",\n    \"HourlyODataCallout\",\n    \"HourlyPublishedPlatformEvents\",\n    \"HourlyPublishedStandardVolumePlatformEvents\",\n    \"HourlyShortTermIdMapping\",\n    \"HourlySyncReportRuns\",\n    \"HourlyTimeBasedWorkflow\",\n    \"MassEmail\",\n    \"MonthlyEinsteinDiscoveryStoryCreation\",\n    \"Package2VersionCreates\",\n    \"Package2VersionCreatesWithoutValidation\",\n    \"PermissionSets\",\n    \"PrivateConnectOutboundCalloutHourlyLimitMB\",\n    \"PublishCallbackUsageInApex\",\n    \"SingleEmail\",\n \
  \   \"StreamingApiConcurrentClients\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Limits\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-limits-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Limits
---
