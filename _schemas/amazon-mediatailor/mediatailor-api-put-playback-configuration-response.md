---
description: PutPlaybackConfigurationResponse schema from Amazon MediaTailor API
layout: schema
name: PutPlaybackConfigurationResponse
properties_list:
- description: ''
  name: AdDecisionServerUrl
  type: object
- description: ''
  name: AvailSuppression
  type: object
- description: ''
  name: Bumper
  type: object
- description: ''
  name: CdnConfiguration
  type: object
- description: ''
  name: ConfigurationAliases
  type: object
- description: ''
  name: DashConfiguration
  type: object
- description: ''
  name: HlsConfiguration
  type: object
- description: ''
  name: LivePreRollConfiguration
  type: object
- description: ''
  name: LogConfiguration
  type: object
- description: ''
  name: ManifestProcessingRules
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: PersonalizationThresholdSeconds
  type: object
- description: ''
  name: PlaybackConfigurationArn
  type: object
- description: ''
  name: PlaybackEndpointPrefix
  type: object
- description: ''
  name: SessionInitializationEndpointPrefix
  type: object
- description: ''
  name: SlateAdUrl
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: TranscodeProfileName
  type: object
- description: ''
  name: VideoContentSourceUrl
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-put-playback-configuration-response-schema.json
slug: mediatailor-api-put-playback-configuration-response
source_filename: mediatailor-api-put-playback-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-put-playback-configuration-response-schema.json\",\n  \"title\": \"PutPlaybackConfigurationResponse\",\n  \"description\": \"PutPlaybackConfigurationResponse schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdDecisionServerUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL for the ad decision server (ADS). This includes the specification of static parameters and placeholders for dynamic parameters. AWS Elemental MediaTailor substitutes player-specific and session-specific parameters as needed when calling the ADS. Alternately, for testing you can provide a static VAST URL. The maximum length is 25,000 characters.\"\n        }\n      ]\n  \
  \  },\n    \"AvailSuppression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailSuppression\"\n        },\n        {\n          \"description\": \"The configuration for avail suppression, also known as ad suppression. For more information about ad suppression, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/ad-behavior.html\\\">Ad Suppression</a>.\"\n        }\n      ]\n    },\n    \"Bumper\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Bumper\"\n        },\n        {\n          \"description\": \"The configuration for bumpers. Bumpers are short audio or video clips that play at the start or before the end of an ad break. To learn more about bumpers, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/bumpers.html\\\">Bumpers</a>.\"\n        }\n      ]\n    },\n    \"CdnConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CdnConfiguration\"\n    \
  \    },\n        {\n          \"description\": \"The configuration for using a content delivery network (CDN), like Amazon CloudFront, for content and ad segment management.\"\n        }\n      ]\n    },\n    \"ConfigurationAliases\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAliasesResponse\"\n        },\n        {\n          \"description\": \"The player parameters and aliases used as dynamic variables during session initialization. For more information, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/variables-domain.html\\\">Domain Variables</a>.\"\n        }\n      ]\n    },\n    \"DashConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DashConfiguration\"\n        },\n        {\n          \"description\": \"The configuration for DASH content.\"\n        }\n      ]\n    },\n    \"HlsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsConfiguration\"\
  \n        },\n        {\n          \"description\": \"The configuration for HLS content.\"\n        }\n      ]\n    },\n    \"LivePreRollConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LivePreRollConfiguration\"\n        },\n        {\n          \"description\": \"The configuration for pre-roll ad insertion.\"\n        }\n      ]\n    },\n    \"LogConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogConfiguration\"\n        },\n        {\n          \"description\": \"The Amazon CloudWatch log settings for a playback configuration.\"\n        }\n      ]\n    },\n    \"ManifestProcessingRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestProcessingRules\"\n        },\n        {\n          \"description\": \"The configuration for manifest processing rules. Manifest processing rules enable customization of the personalized manifests created by MediaTailor.\"\n\
  \        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The identifier for the playback configuration.\"\n        }\n      ]\n    },\n    \"PersonalizationThresholdSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"description\": \"Defines the maximum duration of underfilled ad time (in seconds) allowed in an ad break. If the duration of underfilled ad time exceeds the personalization threshold, then the personalization of the ad break is abandoned and the underlying content is shown. This feature applies to <i>ad replacement</i> in live and VOD streams, rather than ad insertion, because it relies on an underlying content stream. For more information about ad break behavior, including ad replacement and insertion, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/ad-behavior.html\\\
  \">Ad Behavior in AWS Elemental MediaTailor</a>.\"\n        }\n      ]\n    },\n    \"PlaybackConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) associated with the playback configuration.\"\n        }\n      ]\n    },\n    \"PlaybackEndpointPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The playback endpoint prefix associated with the playback configuration.\"\n        }\n      ]\n    },\n    \"SessionInitializationEndpointPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The session initialization endpoint prefix associated with the playback configuration.\"\n        }\n      ]\n    },\n    \"SlateAdUrl\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL for a high-quality video asset to transcode and use to fill in time that's not used by ads. AWS Elemental MediaTailor shows the slate to fill in gaps in media content. Configuring the slate is optional for non-VPAID configurations. For VPAID, the slate is required because MediaTailor provides it in the slots that are designated for dynamic ad content. The slate must be a high-quality asset that contains both audio and video.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags to assign to the playback configuration. Tags are key-value pairs that you can associate with Amazon resources to help with organization, access control, and cost tracking. For more information,\
  \ see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/tagging.html\\\">Tagging AWS Elemental MediaTailor Resources</a>.\"\n        }\n      ]\n    },\n    \"TranscodeProfileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name that is used to associate this playback configuration with a custom transcode profile. This overrides the dynamic transcoding defaults of MediaTailor. Use this only if you have already set up custom profiles with the help of AWS Support.\"\n        }\n      ]\n    },\n    \"VideoContentSourceUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL prefix for the parent manifest for the stream, minus the asset ID. The maximum length is 512 characters.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-put-playback-configuration-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PutPlaybackConfigurationResponse
---
