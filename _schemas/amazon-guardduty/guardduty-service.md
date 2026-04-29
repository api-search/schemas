---
description: Contains additional information about the generated finding.
layout: schema
name: Service
properties_list:
- description: ''
  name: Action
  type: object
- description: ''
  name: Evidence
  type: object
- description: ''
  name: Archived
  type: object
- description: ''
  name: Count
  type: object
- description: ''
  name: DetectorId
  type: object
- description: ''
  name: EventFirstSeen
  type: object
- description: ''
  name: EventLastSeen
  type: object
- description: ''
  name: ResourceRole
  type: object
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: UserFeedback
  type: object
- description: ''
  name: AdditionalInfo
  type: object
- description: ''
  name: FeatureName
  type: object
- description: ''
  name: EbsVolumeScanDetails
  type: object
- description: ''
  name: RuntimeDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-service-schema.json
slug: guardduty-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"Contains additional information about the generated finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Action\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"action\"\n          },\n          \"description\": \"Information about the activity that is described in a finding.\"\n        }\n      ]\n    },\n    \"Evidence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Evidence\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"evidence\"\n          },\n          \"description\": \"An evidence object associated with the service.\"\n        }\n      ]\n\
  \    },\n    \"Archived\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"archived\"\n          },\n          \"description\": \"Indicates whether this finding is archived.\"\n        }\n      ]\n    },\n    \"Count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"count\"\n          },\n          \"description\": \"The total count of the occurrences of this finding type.\"\n        }\n      ]\n    },\n    \"DetectorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"detectorId\"\n          },\n          \"description\": \"The detector ID for the GuardDuty service.\"\n        }\n      ]\n    },\n    \"EventFirstSeen\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"eventFirstSeen\"\n          },\n          \"description\": \"The first-seen timestamp of the activity that prompted GuardDuty to generate this finding.\"\n        }\n      ]\n    },\n    \"EventLastSeen\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"eventLastSeen\"\n          },\n          \"description\": \"The last-seen timestamp of the activity that prompted GuardDuty to generate this finding.\"\n        }\n      ]\n    },\n    \"ResourceRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceRole\"\n          },\n          \"description\": \"The resource role information for this finding.\"\n        }\n      ]\n    },\n    \"ServiceName\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serviceName\"\n          },\n          \"description\": \"The name of the Amazon Web Services service (GuardDuty) that generated a finding.\"\n        }\n      ]\n    },\n    \"UserFeedback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userFeedback\"\n          },\n          \"description\": \"Feedback that was submitted about the finding.\"\n        }\n      ]\n    },\n    \"AdditionalInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceAdditionalInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"additionalInfo\"\n          },\n          \"description\": \"Contains additional information about the generated finding.\"\n        }\n      ]\n    },\n    \"FeatureName\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"featureName\"\n          },\n          \"description\": \"The name of the feature that generated a finding.\"\n        }\n      ]\n    },\n    \"EbsVolumeScanDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbsVolumeScanDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebsVolumeScanDetails\"\n          },\n          \"description\": \"Returns details from the malware scan that created a finding.\"\n        }\n      ]\n    },\n    \"RuntimeDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"runtimeDetails\"\n          },\n          \"description\": \"Information about the process and any required context values for a specific finding\"\n     \
  \   }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-service-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Service
---
