---
description: Use these settings only when you use Kantar watermarking. Specify the values that MediaConvert uses to generate and place Kantar watermarks in your output audio. These settings apply to every output in your job. In addition to specifying these values, you also need to store your Kantar credentials in AWS Secrets Manager. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/kantar-watermarking.html.
layout: schema
name: KantarWatermarkSettings
properties_list:
- description: ''
  name: ChannelName
  type: object
- description: ''
  name: ContentReference
  type: object
- description: ''
  name: CredentialsSecretName
  type: object
- description: ''
  name: FileOffset
  type: object
- description: ''
  name: KantarLicenseId
  type: object
- description: ''
  name: KantarServerUrl
  type: object
- description: ''
  name: LogDestination
  type: object
- description: ''
  name: Metadata3
  type: object
- description: ''
  name: Metadata4
  type: object
- description: ''
  name: Metadata5
  type: object
- description: ''
  name: Metadata6
  type: object
- description: ''
  name: Metadata7
  type: object
- description: ''
  name: Metadata8
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-kantar-watermark-settings-schema.json
slug: mediaconvert-api-kantar-watermark-settings
source_filename: mediaconvert-api-kantar-watermark-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-kantar-watermark-settings-schema.json\",\n  \"title\": \"KantarWatermarkSettings\",\n  \"description\": \"Use these settings only when you use Kantar watermarking. Specify the values that MediaConvert uses to generate and place Kantar watermarks in your output audio. These settings apply to every output in your job. In addition to specifying these values, you also need to store your Kantar credentials in AWS Secrets Manager. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/kantar-watermarking.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max20\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelName\"\n      \
  \    },\n          \"description\": \"Provide an audio channel name from your Kantar audio license.\"\n        }\n      ]\n    },\n    \"ContentReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max50PatternAZAZ09\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"contentReference\"\n          },\n          \"description\": \"Specify a unique identifier for Kantar to use for this piece of content.\"\n        }\n      ]\n    },\n    \"CredentialsSecretName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max512PatternAZAZ09\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"credentialsSecretName\"\n          },\n          \"description\": \"Provide the name of the AWS Secrets Manager secret where your Kantar credentials are stored. Note that your MediaConvert service role must provide access to this secret. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/granting-permissions-for-mediaconvert-to-access-secrets-manager-secret.html.\
  \ For instructions on creating a secret, see https://docs.aws.amazon.com/secretsmanager/latest/userguide/tutorials_basic.html, in the AWS Secrets Manager User Guide.\"\n        }\n      ]\n    },\n    \"FileOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fileOffset\"\n          },\n          \"description\": \"Optional. Specify an offset, in whole seconds, from the start of your output and the beginning of the watermarking. When you don't specify an offset, Kantar defaults to zero.\"\n        }\n      ]\n    },\n    \"KantarLicenseId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kantarLicenseId\"\n          },\n          \"description\": \"Provide your Kantar license ID number. You should get this number from Kantar.\"\n        }\n \
  \     ]\n    },\n    \"KantarServerUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternHttpsKantarmediaCom\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kantarServerUrl\"\n          },\n          \"description\": \"Provide the HTTPS endpoint to the Kantar server. You should get this endpoint from Kantar.\"\n        }\n      ]\n    },\n    \"LogDestination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternS3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"logDestination\"\n          },\n          \"description\": \"Optional. Specify the Amazon S3 bucket where you want MediaConvert to store your Kantar watermark XML logs. When you don't specify a bucket, MediaConvert doesn't save these logs. Note that your MediaConvert service role must provide access to this location. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/iam-role.html\"\
  \n        }\n      ]\n    },\n    \"Metadata3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadata3\"\n          },\n          \"description\": \"You can optionally use this field to specify the first timestamp that Kantar embeds during watermarking. Kantar suggests that you be very cautious when using this Kantar feature, and that you use it only on channels that are managed specifically for use with this feature by your Audience Measurement Operator. For more information about this feature, contact Kantar technical support.\"\n        }\n      ]\n    },\n    \"Metadata4\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadata4\"\n          },\n          \"description\": \"Additional metadata that MediaConvert sends to Kantar. Maximum length\
  \ is 50 characters.\"\n        }\n      ]\n    },\n    \"Metadata5\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadata5\"\n          },\n          \"description\": \"Additional metadata that MediaConvert sends to Kantar. Maximum length is 50 characters.\"\n        }\n      ]\n    },\n    \"Metadata6\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadata6\"\n          },\n          \"description\": \"Additional metadata that MediaConvert sends to Kantar. Maximum length is 50 characters.\"\n        }\n      ]\n    },\n    \"Metadata7\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadata7\"\n          },\n          \"description\"\
  : \"Additional metadata that MediaConvert sends to Kantar. Maximum length is 50 characters.\"\n        }\n      ]\n    },\n    \"Metadata8\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadata8\"\n          },\n          \"description\": \"Additional metadata that MediaConvert sends to Kantar. Maximum length is 50 characters.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-kantar-watermark-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: KantarWatermarkSettings
---
