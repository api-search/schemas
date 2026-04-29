---
description: <important> <p>Outputs recommended instead.</p> </important> <p>If you specified one output for a job, information about that output. If you specified multiple outputs for a job, the <code>Output</code> object lists information about the first output. This duplicates the information that is listed for the first output in the <code>Outputs</code> object.</p>
layout: schema
name: JobOutput
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: ThumbnailPattern
  type: object
- description: ''
  name: ThumbnailEncryption
  type: object
- description: ''
  name: Rotate
  type: object
- description: ''
  name: PresetId
  type: object
- description: ''
  name: SegmentDuration
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusDetail
  type: object
- description: ''
  name: Duration
  type: object
- description: ''
  name: Width
  type: object
- description: ''
  name: Height
  type: object
- description: ''
  name: FrameRate
  type: object
- description: ''
  name: FileSize
  type: object
- description: ''
  name: DurationMillis
  type: object
- description: ''
  name: Watermarks
  type: object
- description: ''
  name: AlbumArt
  type: object
- description: ''
  name: Composition
  type: object
- description: ''
  name: Captions
  type: object
- description: ''
  name: Encryption
  type: object
- description: ''
  name: AppliedColorSpaceConversion
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-job-output-schema.json
slug: amazon-elastic-transcoder-job-output
source_filename: amazon-elastic-transcoder-job-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-job-output-schema.json\",\n  \"title\": \"JobOutput\",\n  \"description\": \"<important> <p>Outputs recommended instead.</p> </important> <p>If you specified one output for a job, information about that output. If you specified multiple outputs for a job, the <code>Output</code> object lists information about the first output. This duplicates the information that is listed for the first output in the <code>Outputs</code> object.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A sequential counter, starting with 1, that identifies an output among the outputs from the current job. In the Output syntax, this value is\
  \ always 1.\"\n        }\n      ]\n    },\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Key\"\n        },\n        {\n          \"description\": \" The name to assign to the transcoded file. Elastic Transcoder saves the file in the Amazon S3 bucket specified by the <code>OutputBucket</code> object in the pipeline that is specified by the pipeline ID.\"\n        }\n      ]\n    },\n    \"ThumbnailPattern\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThumbnailPattern\"\n        },\n        {\n          \"description\": \"<p>Whether you want Elastic Transcoder to create thumbnails for your videos and, if so, how you want Elastic Transcoder to name the files.</p> <p>If you don't want Elastic Transcoder to create thumbnails, specify \\\"\\\".</p> <p>If you do want Elastic Transcoder to create thumbnails, specify the information that you want to include in the file name for each thumbnail. You can specify the following\
  \ values in any sequence:</p> <ul> <li> <p> <b> <code>{count}</code> (Required)</b>: If you want to create thumbnails, you must include <code>{count}</code> in the <code>ThumbnailPattern</code> object. Wherever you specify <code>{count}</code>, Elastic Transcoder adds a five-digit sequence number (beginning with <b>00001</b>) to thumbnail file names. The number indicates where a given thumbnail appears in the sequence of thumbnails for a transcoded file. </p> <important> <p>If you specify a literal value and/or <code>{resolution}</code> but you omit <code>{count}</code>, Elastic Transcoder returns a validation error and does not create the job.</p> </important> </li> <li> <p> <b>Literal values (Optional)</b>: You can specify literal values anywhere in the <code>ThumbnailPattern</code> object. For example, you can include them as a file name prefix or as a delimiter between <code>{resolution}</code> and <code>{count}</code>. </p> </li> <li> <p> <b> <code>{resolution}</code> (Optional)</b>:\
  \ If you want Elastic Transcoder to include the resolution in the file name, include <code>{resolution}</code> in the <code>ThumbnailPattern</code> object. </p> </li> </ul> <p>When creating thumbnails, Elastic Transcoder automatically saves the files in the format (.jpg or .png) that appears in the preset that you specified in the <code>PresetID</code> value of <code>CreateJobOutput</code>. Elastic Transcoder also appends the applicable file name extension.</p>\"\n        }\n      ]\n    },\n    \"ThumbnailEncryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n        {\n          \"description\": \"The encryption settings, if any, that you want Elastic Transcoder to apply to your thumbnail.\"\n        }\n      ]\n    },\n    \"Rotate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rotate\"\n        },\n        {\n          \"description\": \"<p>The number of degrees clockwise by which you want\
  \ Elastic Transcoder to rotate the output relative to the input. Enter one of the following values:</p> <p> <code>auto</code>, <code>0</code>, <code>90</code>, <code>180</code>, <code>270</code> </p> <p> The value <code>auto</code> generally works only if the file that you're transcoding contains rotation metadata.</p>\"\n        }\n      ]\n    },\n    \"PresetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The value of the <code>Id</code> object for the preset that you want to use for this job. The preset determines the audio, video, and thumbnail settings that Elastic Transcoder uses for transcoding. To use a preset that you created, specify the preset ID that Elastic Transcoder returned in the response when you created the preset. You can also use the Elastic Transcoder system presets, which you can get with <code>ListPresets</code>.\"\n        }\n      ]\n    },\n    \"SegmentDuration\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FloatString\"\n        },\n        {\n          \"description\": \"<important> <p>(Outputs in Fragmented MP4 or MPEG-TS format only.</p> </important> <p>If you specify a preset in <code>PresetId</code> for which the value of <code>Container</code> is <code>fmp4</code> (Fragmented MP4) or <code>ts</code> (MPEG-TS), <code>SegmentDuration</code> is the target maximum duration of each segment in seconds. For <code>HLSv3</code> format playlists, each media segment is stored in a separate <code>.ts</code> file. For <code>HLSv4</code>, <code>MPEG-DASH</code>, and <code>Smooth</code> playlists, all media segments for an output are stored in a single file. Each segment is approximately the length of the <code>SegmentDuration</code>, though individual segments might be shorter or longer.</p> <p>The range of valid values is 1 to 60 seconds. If the duration of the video is not evenly divisible by <code>SegmentDuration</code>,\
  \ the duration of the last segment is the remainder of total length/SegmentDuration.</p> <p>Elastic Transcoder creates an output-specific playlist for each output <code>HLS</code> output that you specify in OutputKeys. To add an output to the master playlist for this job, include it in the <code>OutputKeys</code> of the associated playlist.</p>\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"<p> The status of one output in a job. If you specified only one output for the job, <code>Outputs:Status</code> is always the same as <code>Job:Status</code>. If you specified more than one output: </p> <ul> <li> <p> <code>Job:Status</code> and <code>Outputs:Status</code> for all of the outputs is Submitted until Elastic Transcoder starts to process the first output.</p> </li> <li> <p>When Elastic Transcoder starts to process the first output, <code>Outputs:Status</code>\
  \ for that output and <code>Job:Status</code> both change to Progressing. For each output, the value of <code>Outputs:Status</code> remains Submitted until Elastic Transcoder starts to process the output.</p> </li> <li> <p>Job:Status remains Progressing until all of the outputs reach a terminal status, either Complete or Error.</p> </li> <li> <p>When all of the outputs reach a terminal status, <code>Job:Status</code> changes to Complete only if <code>Outputs:Status</code> for all of the outputs is <code>Complete</code>. If <code>Outputs:Status</code> for one or more outputs is <code>Error</code>, the terminal status for <code>Job:Status</code> is also <code>Error</code>.</p> </li> </ul> <p>The value of <code>Status</code> is one of the following: <code>Submitted</code>, <code>Progressing</code>, <code>Complete</code>, <code>Canceled</code>, or <code>Error</code>. </p>\"\n        }\n      ]\n    },\n    \"StatusDetail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\
  \n        },\n        {\n          \"description\": \"Information that further explains <code>Status</code>.\"\n        }\n      ]\n    },\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"Duration of the output file, in seconds.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"Specifies the width of the output file in pixels.\"\n        }\n      ]\n    },\n    \"Height\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"Height of the output file, in pixels.\"\n        }\n      ]\n    },\n    \"FrameRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FloatString\"\n        },\n        {\n          \"description\"\
  : \"Frame rate of the output file, in frames per second.\"\n        }\n      ]\n    },\n    \"FileSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"File size of the output file, in bytes.\"\n        }\n      ]\n    },\n    \"DurationMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"Duration of the output file, in milliseconds.\"\n        }\n      ]\n    },\n    \"Watermarks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobWatermarks\"\n        },\n        {\n          \"description\": \"<p>Information about the watermarks that you want Elastic Transcoder to add to the video during transcoding. You can specify up to four watermarks for each output. Settings for each watermark must be defined in the preset that you specify in <code>Preset</code> for\
  \ the current output.</p> <p>Watermarks are added to the output video in the sequence in which you list them in the job output\\u2014the first watermark in the list is added to the output video first, the second watermark in the list is added next, and so on. As a result, if the settings in a preset cause Elastic Transcoder to place all watermarks in the same location, the second watermark that you add covers the first one, the third one covers the second, and the fourth one covers the third.</p>\"\n        }\n      ]\n    },\n    \"AlbumArt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobAlbumArt\"\n        },\n        {\n          \"description\": \"The album art to be associated with the output file, if any.\"\n        }\n      ]\n    },\n    \"Composition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Composition\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"You can create\
  \ an output file that contains an excerpt from the input file. This excerpt, called a clip, can come from the beginning, middle, or end of the file. The Composition object contains settings for the clips that make up an output file. For the current release, you can only specify settings for a single clip per output file. The Composition object cannot be null.\"\n        }\n      ]\n    },\n    \"Captions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Captions\"\n        },\n        {\n          \"description\": \"<p>You can configure Elastic Transcoder to transcode captions, or subtitles, from one format to another. All captions must be in UTF-8. Elastic Transcoder supports two types of captions:</p> <ul> <li> <p> <b>Embedded:</b> Embedded captions are included in the same file as the audio and video. Elastic Transcoder supports only one embedded caption per language, to a maximum of 300 embedded captions per file.</p> <p>Valid input values include: <code>CEA-608\
  \ (EIA-608</code>, first non-empty channel only), <code>CEA-708 (EIA-708</code>, first non-empty channel only), and <code>mov-text</code> </p> <p>Valid outputs include: <code>mov-text</code> </p> <p>Elastic Transcoder supports a maximum of one embedded format per output.</p> </li> <li> <p> <b>Sidecar:</b> Sidecar captions are kept in a separate metadata file from the audio and video data. Sidecar captions require a player that is capable of understanding the relationship between the video file and the sidecar file. Elastic Transcoder supports only one sidecar caption per language, to a maximum of 20 sidecar captions per file.</p> <p>Valid input values include: <code>dfxp</code> (first div element only), <code>ebu-tt</code>, <code>scc</code>, <code>smpt</code>, <code>srt</code>, <code>ttml</code> (first div element only), and <code>webvtt</code> </p> <p>Valid outputs include: <code>dfxp</code> (first div element only), <code>scc</code>, <code>srt</code>, and <code>webvtt</code>.</p> </li>\
  \ </ul> <p>If you want ttml or smpte-tt compatible captions, specify dfxp as your output format.</p> <p>Elastic Transcoder does not support OCR (Optical Character Recognition), does not accept pictures as a valid input for captions, and is not available for audio-only transcoding. Elastic Transcoder does not preserve text formatting (for example, italics) during the transcoding process.</p> <p>To remove captions or leave the captions empty, set <code>Captions</code> to null. To pass through existing captions unchanged, set the <code>MergePolicy</code> to <code>MergeRetain</code>, and pass in a null <code>CaptionSources</code> array.</p> <p>For more information on embedded files, see the Subtitles Wikipedia page.</p> <p>For more information on sidecar files, see the Extensible Metadata Platform and Sidecar file Wikipedia pages.</p>\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n  \
  \      {\n          \"description\": \"The encryption settings, if any, that you want Elastic Transcoder to apply to your output files. If you choose to use encryption, you must specify a mode to use. If you choose not to use encryption, Elastic Transcoder writes an unencrypted file to your Amazon S3 bucket.\"\n        }\n      ]\n    },\n    \"AppliedColorSpaceConversion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"If Elastic Transcoder used a preset with a <code>ColorSpaceConversionMode</code> to transcode the output file, the <code>AppliedColorSpaceConversion</code> parameter shows the conversion used. If no <code>ColorSpaceConversionMode</code> was defined in the preset, this parameter is not be included in the job response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-job-output-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: JobOutput
---
