---
description: A Dynamic Adaptive Streaming over HTTP (DASH) packaging configuration.
layout: schema
name: DashPackage
properties_list:
- description: ''
  name: AdTriggers
  type: object
- description: ''
  name: AdsOnDeliveryRestrictions
  type: object
- description: ''
  name: Encryption
  type: object
- description: ''
  name: IncludeIframeOnlyStream
  type: object
- description: ''
  name: ManifestLayout
  type: object
- description: ''
  name: ManifestWindowSeconds
  type: object
- description: ''
  name: MinBufferTimeSeconds
  type: object
- description: ''
  name: MinUpdatePeriodSeconds
  type: object
- description: ''
  name: PeriodTriggers
  type: object
- description: ''
  name: Profile
  type: object
- description: ''
  name: SegmentDurationSeconds
  type: object
- description: ''
  name: SegmentTemplateFormat
  type: object
- description: ''
  name: StreamSelection
  type: object
- description: ''
  name: SuggestedPresentationDelaySeconds
  type: object
- description: ''
  name: UtcTiming
  type: object
- description: ''
  name: UtcTimingUri
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-dash-package-schema.json
slug: mediapackage-api-dash-package
source_filename: mediapackage-api-dash-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-dash-package-schema.json\",\n  \"title\": \"DashPackage\",\n  \"description\": \"A Dynamic Adaptive Streaming over HTTP (DASH) packaging configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdTriggers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdTriggers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adTriggers\"\n          }\n        }\n      ]\n    },\n    \"AdsOnDeliveryRestrictions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdsOnDeliveryRestrictions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adsOnDeliveryRestrictions\"\n          }\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/DashEncryption\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryption\"\n          }\n        }\n      ]\n    },\n    \"IncludeIframeOnlyStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"includeIframeOnlyStream\"\n          },\n          \"description\": \"When enabled, an I-Frame only stream will be included in the output.\"\n        }\n      ]\n    },\n    \"ManifestLayout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestLayout\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestLayout\"\n          },\n          \"description\": \"Determines the position of some tags in the Media Presentation Description (MPD).  When set to FULL, elements like SegmentTemplate and ContentProtection are included in each Representation.  When set to COMPACT, duplicate elements\
  \ are combined and presented at the AdaptationSet level.\"\n        }\n      ]\n    },\n    \"ManifestWindowSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestWindowSeconds\"\n          },\n          \"description\": \"Time window (in seconds) contained in each manifest.\"\n        }\n      ]\n    },\n    \"MinBufferTimeSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minBufferTimeSeconds\"\n          },\n          \"description\": \"Minimum duration (in seconds) that a player will buffer media before starting the presentation.\"\n        }\n      ]\n    },\n    \"MinUpdatePeriodSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"minUpdatePeriodSeconds\"\n          },\n          \"description\": \"Minimum duration (in seconds) between potential changes to the Dynamic Adaptive Streaming over HTTP (DASH) Media Presentation Description (MPD).\"\n        }\n      ]\n    },\n    \"PeriodTriggers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__PeriodTriggersElement\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"periodTriggers\"\n          },\n          \"description\": \"A list of triggers that controls when the outgoing Dynamic Adaptive Streaming over HTTP (DASH)\\nMedia Presentation Description (MPD) will be partitioned into multiple periods. If empty, the content will not\\nbe partitioned into more than one period. If the list contains \\\"ADS\\\", new periods will be created where\\nthe Channel source contains SCTE-35 ad markers.\\n\"\n        }\n      ]\n    },\n    \"Profile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Profile\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"profile\"\n          },\n          \"description\": \"The Dynamic Adaptive Streaming over HTTP (DASH) profile type.  When set to \\\"HBBTV_1_5\\\", HbbTV 1.5 compliant output is enabled. When set to \\\"DVB-DASH_2014\\\", DVB-DASH 2014 compliant output is enabled.\"\n        }\n      ]\n    },\n    \"SegmentDurationSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentDurationSeconds\"\n          },\n          \"description\": \"Duration (in seconds) of each segment. Actual segments will be\\nrounded to the nearest multiple of the source segment duration.\\n\"\n        }\n      ]\n    },\n    \"SegmentTemplateFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentTemplateFormat\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentTemplateFormat\"\
  \n          },\n          \"description\": \"Determines the type of SegmentTemplate included in the Media Presentation Description (MPD).  When set to NUMBER_WITH_TIMELINE, a full timeline is presented in each SegmentTemplate, with $Number$ media URLs.  When set to TIME_WITH_TIMELINE, a full timeline is presented in each SegmentTemplate, with $Time$ media URLs. When set to NUMBER_WITH_DURATION, only a duration is included in each SegmentTemplate, with $Number$ media URLs.\"\n        }\n      ]\n    },\n    \"StreamSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamSelection\"\n          }\n        }\n      ]\n    },\n    \"SuggestedPresentationDelaySeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"suggestedPresentationDelaySeconds\"\n  \
  \        },\n          \"description\": \"Duration (in seconds) to delay live content before presentation.\"\n        }\n      ]\n    },\n    \"UtcTiming\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UtcTiming\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"utcTiming\"\n          },\n          \"description\": \"Determines the type of UTCTiming included in the Media Presentation Description (MPD)\"\n        }\n      ]\n    },\n    \"UtcTimingUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"utcTimingUri\"\n          },\n          \"description\": \"Specifies the value attribute of the UTCTiming field when utcTiming is set to HTTP-ISO, HTTP-HEAD or HTTP-XSDATE\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-dash-package-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DashPackage
---
