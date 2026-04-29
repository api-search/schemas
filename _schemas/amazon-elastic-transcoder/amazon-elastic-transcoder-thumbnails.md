---
description: Thumbnails for videos.
layout: schema
name: Thumbnails
properties_list:
- description: ''
  name: Format
  type: object
- description: ''
  name: Interval
  type: object
- description: ''
  name: Resolution
  type: object
- description: ''
  name: AspectRatio
  type: object
- description: ''
  name: MaxWidth
  type: object
- description: ''
  name: MaxHeight
  type: object
- description: ''
  name: SizingPolicy
  type: object
- description: ''
  name: PaddingPolicy
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-thumbnails-schema.json
slug: amazon-elastic-transcoder-thumbnails
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-thumbnails-schema.json\",\n  \"title\": \"Thumbnails\",\n  \"description\": \"Thumbnails for videos.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JpgOrPng\"\n        },\n        {\n          \"description\": \"<p>The format of thumbnails, if any. Valid values are <code>jpg</code> and <code>png</code>. </p> <p>You specify whether you want Elastic Transcoder to create thumbnails when you create a job.</p>\"\n        }\n      ]\n    },\n    \"Interval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Digits\"\n        },\n        {\n          \"description\": \"The approximate number of seconds between thumbnails. Specify an integer value.\"\n\
  \        }\n      ]\n    },\n    \"Resolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThumbnailResolution\"\n        },\n        {\n          \"description\": \"<important> <p>To better control resolution and aspect ratio of thumbnails, we recommend that you use the values <code>MaxWidth</code>, <code>MaxHeight</code>, <code>SizingPolicy</code>, and <code>PaddingPolicy</code> instead of <code>Resolution</code> and <code>AspectRatio</code>. The two groups of settings are mutually exclusive. Do not use them together.</p> </important> <p>The width and height of thumbnail files in pixels. Specify a value in the format <code> <i>width</i> </code> x <code> <i>height</i> </code> where both values are even integers. The values cannot exceed the width and height that you specified in the <code>Video:Resolution</code> object.</p>\"\n        }\n      ]\n    },\n    \"AspectRatio\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AspectRatio\"\
  \n        },\n        {\n          \"description\": \"<important> <p>To better control resolution and aspect ratio of thumbnails, we recommend that you use the values <code>MaxWidth</code>, <code>MaxHeight</code>, <code>SizingPolicy</code>, and <code>PaddingPolicy</code> instead of <code>Resolution</code> and <code>AspectRatio</code>. The two groups of settings are mutually exclusive. Do not use them together.</p> </important> <p>The aspect ratio of thumbnails. Valid values include:</p> <p> <code>auto</code>, <code>1:1</code>, <code>4:3</code>, <code>3:2</code>, <code>16:9</code> </p> <p>If you specify <code>auto</code>, Elastic Transcoder tries to preserve the aspect ratio of the video in the output file.</p>\"\n        }\n      ]\n    },\n    \"MaxWidth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DigitsOrAuto\"\n        },\n        {\n          \"description\": \"The maximum width of thumbnails in pixels. If you specify auto, Elastic Transcoder uses\
  \ 1920 (Full HD) as the default value. If you specify a numeric value, enter an even integer between 32 and 4096.\"\n        }\n      ]\n    },\n    \"MaxHeight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DigitsOrAuto\"\n        },\n        {\n          \"description\": \"The maximum height of thumbnails in pixels. If you specify auto, Elastic Transcoder uses 1080 (Full HD) as the default value. If you specify a numeric value, enter an even integer between 32 and 3072.\"\n        }\n      ]\n    },\n    \"SizingPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SizingPolicy\"\n        },\n        {\n          \"description\": \"<p>Specify one of the following values to control scaling of thumbnails:</p> <ul> <li> <p> <code>Fit</code>: Elastic Transcoder scales thumbnails so they match the value that you specified in thumbnail MaxWidth or MaxHeight settings without exceeding the other value. </p> </li> <li> <p> <code>Fill</code>:\
  \ Elastic Transcoder scales thumbnails so they match the value that you specified in thumbnail <code>MaxWidth</code> or <code>MaxHeight</code> settings and matches or exceeds the other value. Elastic Transcoder centers the image in thumbnails and then crops in the dimension (if any) that exceeds the maximum value.</p> </li> <li> <p> <code>Stretch</code>: Elastic Transcoder stretches thumbnails to match the values that you specified for thumbnail <code>MaxWidth</code> and <code>MaxHeight</code> settings. If the relative proportions of the input video and thumbnails are different, the thumbnails will be distorted.</p> </li> <li> <p> <code>Keep</code>: Elastic Transcoder does not scale thumbnails. If either dimension of the input video exceeds the values that you specified for thumbnail <code>MaxWidth</code> and <code>MaxHeight</code> settings, Elastic Transcoder crops the thumbnails.</p> </li> <li> <p> <code>ShrinkToFit</code>: Elastic Transcoder scales thumbnails down so that their dimensions\
  \ match the values that you specified for at least one of thumbnail <code>MaxWidth</code> and <code>MaxHeight</code> without exceeding either value. If you specify this option, Elastic Transcoder does not scale thumbnails up.</p> </li> <li> <p> <code>ShrinkToFill</code>: Elastic Transcoder scales thumbnails down so that their dimensions match the values that you specified for at least one of <code>MaxWidth</code> and <code>MaxHeight</code> without dropping below either value. If you specify this option, Elastic Transcoder does not scale thumbnails up.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"PaddingPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaddingPolicy\"\n        },\n        {\n          \"description\": \"When you set <code>PaddingPolicy</code> to <code>Pad</code>, Elastic Transcoder may add black bars to the top and bottom and/or left and right sides of thumbnails to make the total size of the thumbnails match the values that\
  \ you specified for thumbnail <code>MaxWidth</code> and <code>MaxHeight</code> settings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-thumbnails-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: Thumbnails
---
