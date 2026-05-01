---
description: Contains information about a malware scan.
layout: schema
name: Scan
properties_list:
- description: ''
  name: DetectorId
  type: object
- description: ''
  name: AdminDetectorId
  type: object
- description: ''
  name: ScanId
  type: object
- description: ''
  name: ScanStatus
  type: object
- description: ''
  name: FailureReason
  type: object
- description: ''
  name: ScanStartTime
  type: object
- description: ''
  name: ScanEndTime
  type: object
- description: ''
  name: TriggerDetails
  type: object
- description: ''
  name: ResourceDetails
  type: object
- description: ''
  name: ScanResultDetails
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: TotalBytes
  type: object
- description: ''
  name: FileCount
  type: object
- description: ''
  name: AttachedVolumes
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-schema.json
slug: guardduty-scan
source_filename: guardduty-scan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-schema.json\",\n  \"title\": \"Scan\",\n  \"description\": \"Contains information about a malware scan.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DetectorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"detectorId\"\n          },\n          \"description\": \"The unique ID of the detector that the request is associated with.\"\n        }\n      ]\n    },\n    \"AdminDetectorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adminDetectorId\"\n          },\n          \"description\": \"The unique detector ID of the administrator account that the\
  \ request is associated with. Note that this value will be the same as the one used for <code>DetectorId</code> if the account is an administrator.\"\n        }\n      ]\n    },\n    \"ScanId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanId\"\n          },\n          \"description\": \"The unique scan ID associated with a scan entry.\"\n        }\n      ]\n    },\n    \"ScanStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanStatus\"\n          },\n          \"description\": \"An enum value representing possible scan statuses.\"\n        }\n      ]\n    },\n    \"FailureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"failureReason\"\
  \n          },\n          \"description\": \"Represents the reason for FAILED scan status.\"\n        }\n      ]\n    },\n    \"ScanStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanStartTime\"\n          },\n          \"description\": \"The timestamp of when the scan was triggered.\"\n        }\n      ]\n    },\n    \"ScanEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanEndTime\"\n          },\n          \"description\": \"The timestamp of when the scan was finished.\"\n        }\n      ]\n    },\n    \"TriggerDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"triggerDetails\"\n          },\n          \"description\"\
  : \"Specifies the reason why the scan was initiated.\"\n        }\n      ]\n    },\n    \"ResourceDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceDetails\"\n          },\n          \"description\": \"Represents the resources that were scanned in the scan entry.\"\n        }\n      ]\n    },\n    \"ScanResultDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanResultDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanResultDetails\"\n          },\n          \"description\": \"Represents the result of the scan.\"\n        }\n      ]\n    },\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The ID for the\
  \ account that belongs to the scan.\"\n        }\n      ]\n    },\n    \"TotalBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveLong\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"totalBytes\"\n          },\n          \"description\": \"Represents total bytes that were scanned.\"\n        }\n      ]\n    },\n    \"FileCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveLong\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fileCount\"\n          },\n          \"description\": \"Represents the number of files that were scanned.\"\n        }\n      ]\n    },\n    \"AttachedVolumes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attachedVolumes\"\n          },\n          \"description\": \"List of volumes that were attached to the original instance\
  \ to be scanned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Scan
---
