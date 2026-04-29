---
description: Information about the file that you're transcoding.
layout: schema
name: JobInput
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: FrameRate
  type: object
- description: ''
  name: Resolution
  type: object
- description: ''
  name: AspectRatio
  type: object
- description: ''
  name: Interlaced
  type: object
- description: ''
  name: Container
  type: object
- description: ''
  name: Encryption
  type: object
- description: ''
  name: TimeSpan
  type: object
- description: ''
  name: InputCaptions
  type: object
- description: ''
  name: DetectedProperties
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-job-input-schema.json
slug: amazon-elastic-transcoder-job-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-job-input-schema.json\",\n  \"title\": \"JobInput\",\n  \"description\": \"Information about the file that you're transcoding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongKey\"\n        },\n        {\n          \"description\": \"<p> The name of the file to transcode. Elsewhere in the body of the JSON block is the the ID of the pipeline to use for processing the job. The <code>InputBucket</code> object in that pipeline tells Elastic Transcoder which Amazon S3 bucket to get the file from. </p> <p>If the file name includes a prefix, such as <code>cooking/lasagna.mpg</code>, include the prefix in the key. If the file isn't in the specified bucket, Elastic Transcoder returns\
  \ an error.</p>\"\n        }\n      ]\n    },\n    \"FrameRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameRate\"\n        },\n        {\n          \"description\": \"<p>The frame rate of the input file. If you want Elastic Transcoder to automatically detect the frame rate of the input file, specify <code>auto</code>. If you want to specify the frame rate for the input file, enter one of the following values: </p> <p> <code>10</code>, <code>15</code>, <code>23.97</code>, <code>24</code>, <code>25</code>, <code>29.97</code>, <code>30</code>, <code>60</code> </p> <p>If you specify a value other than <code>auto</code>, Elastic Transcoder disables automatic detection of the frame rate.</p>\"\n        }\n      ]\n    },\n    \"Resolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Resolution\"\n        },\n        {\n          \"description\": \"This value must be <code>auto</code>, which causes Elastic Transcoder\
  \ to automatically detect the resolution of the input file.\"\n        }\n      ]\n    },\n    \"AspectRatio\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AspectRatio\"\n        },\n        {\n          \"description\": \"<p> The aspect ratio of the input file. If you want Elastic Transcoder to automatically detect the aspect ratio of the input file, specify <code>auto</code>. If you want to specify the aspect ratio for the output file, enter one of the following values: </p> <p> <code>1:1</code>, <code>4:3</code>, <code>3:2</code>, <code>16:9</code> </p> <p> If you specify a value other than <code>auto</code>, Elastic Transcoder disables automatic detection of the aspect ratio. </p>\"\n        }\n      ]\n    },\n    \"Interlaced\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Interlaced\"\n        },\n        {\n          \"description\": \"<p>Whether the input file is interlaced. If you want Elastic Transcoder to automatically\
  \ detect whether the input file is interlaced, specify <code>auto</code>. If you want to specify whether the input file is interlaced, enter one of the following values:</p> <p> <code>true</code>, <code>false</code> </p> <p>If you specify a value other than <code>auto</code>, Elastic Transcoder disables automatic detection of interlacing.</p>\"\n        }\n      ]\n    },\n    \"Container\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobContainer\"\n        },\n        {\n          \"description\": \"<p>The container type for the input file. If you want Elastic Transcoder to automatically detect the container type of the input file, specify <code>auto</code>. If you want to specify the container type for the input file, enter one of the following values: </p> <p> <code>3gp</code>, <code>aac</code>, <code>asf</code>, <code>avi</code>, <code>divx</code>, <code>flv</code>, <code>m4a</code>, <code>mkv</code>, <code>mov</code>, <code>mp3</code>, <code>mp4</code>,\
  \ <code>mpeg</code>, <code>mpeg-ps</code>, <code>mpeg-ts</code>, <code>mxf</code>, <code>ogg</code>, <code>vob</code>, <code>wav</code>, <code>webm</code> </p>\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n        {\n          \"description\": \"The encryption settings, if any, that are used for decrypting your input files. If your input file is encrypted, you must specify the mode that Elastic Transcoder uses to decrypt your file.\"\n        }\n      ]\n    },\n    \"TimeSpan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSpan\"\n        },\n        {\n          \"description\": \"Settings for clipping an input. Each input can have different clip settings.\"\n        }\n      ]\n    },\n    \"InputCaptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputCaptions\"\n        },\n        {\n          \"description\"\
  : \"<p>You can configure Elastic Transcoder to transcode captions, or subtitles, from one format to another. All captions must be in UTF-8. Elastic Transcoder supports two types of captions:</p> <ul> <li> <p> <b>Embedded:</b> Embedded captions are included in the same file as the audio and video. Elastic Transcoder supports only one embedded caption per language, to a maximum of 300 embedded captions per file.</p> <p>Valid input values include: <code>CEA-608 (EIA-608</code>, first non-empty channel only), <code>CEA-708 (EIA-708</code>, first non-empty channel only), and <code>mov-text</code> </p> <p>Valid outputs include: <code>mov-text</code> </p> <p>Elastic Transcoder supports a maximum of one embedded format per output.</p> </li> <li> <p> <b>Sidecar:</b> Sidecar captions are kept in a separate metadata file from the audio and video data. Sidecar captions require a player that is capable of understanding the relationship between the video file and the sidecar file. Elastic Transcoder\
  \ supports only one sidecar caption per language, to a maximum of 20 sidecar captions per file.</p> <p>Valid input values include: <code>dfxp</code> (first div element only), <code>ebu-tt</code>, <code>scc</code>, <code>smpt</code>, <code>srt</code>, <code>ttml</code> (first div element only), and <code>webvtt</code> </p> <p>Valid outputs include: <code>dfxp</code> (first div element only), <code>scc</code>, <code>srt</code>, and <code>webvtt</code>.</p> </li> </ul> <p>If you want ttml or smpte-tt compatible captions, specify dfxp as your output format.</p> <p>Elastic Transcoder does not support OCR (Optical Character Recognition), does not accept pictures as a valid input for captions, and is not available for audio-only transcoding. Elastic Transcoder does not preserve text formatting (for example, italics) during the transcoding process.</p> <p>To remove captions or leave the captions empty, set <code>Captions</code> to null. To pass through existing captions unchanged, set the <code>MergePolicy</code>\
  \ to <code>MergeRetain</code>, and pass in a null <code>CaptionSources</code> array.</p> <p>For more information on embedded files, see the Subtitles Wikipedia page.</p> <p>For more information on sidecar files, see the Extensible Metadata Platform and Sidecar file Wikipedia pages.</p>\"\n        }\n      ]\n    },\n    \"DetectedProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedProperties\"\n        },\n        {\n          \"description\": \"The detected properties of the input file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-job-input-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: JobInput
---
