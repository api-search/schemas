---
description: A section of the response body that provides information about the job that is created.
layout: schema
name: Job
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: PipelineId
  type: object
- description: ''
  name: Input
  type: object
- description: ''
  name: Inputs
  type: object
- description: ''
  name: Output
  type: object
- description: ''
  name: Outputs
  type: object
- description: ''
  name: OutputKeyPrefix
  type: object
- description: ''
  name: Playlists
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: UserMetadata
  type: object
- description: ''
  name: Timing
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-job-schema.json
slug: amazon-elastic-transcoder-job
source_filename: amazon-elastic-transcoder-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"A section of the response body that provides information about the job that is created.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The identifier that Elastic Transcoder assigned to the job. You use this value to get settings for the job or to delete the job.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the job.\"\n        }\n      ]\n    },\n    \"PipelineId\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \" The <code>Id</code> of the pipeline that you want Elastic Transcoder to use for transcoding. The pipeline determines several settings, including the Amazon S3 bucket from which Elastic Transcoder gets the files to transcode and the bucket into which Elastic Transcoder puts the transcoded files. \"\n        }\n      ]\n    },\n    \"Input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobInput\"\n        },\n        {\n          \"description\": \"A section of the request or response body that provides information about the file that is being transcoded.\"\n        }\n      ]\n    },\n    \"Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobInputs\"\n        },\n        {\n          \"description\": \"Information about the files that you're transcoding. If you specified multiple files for this job, Elastic\
  \ Transcoder stitches the files together to make one output.\"\n        }\n      ]\n    },\n    \"Output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobOutput\"\n        },\n        {\n          \"description\": \"<p>If you specified one output for a job, information about that output. If you specified multiple outputs for a job, the Output object lists information about the first output. This duplicates the information that is listed for the first output in the Outputs object.</p> <important> <p>Outputs recommended instead.</p> </important> <p>A section of the request or response body that provides information about the transcoded (target) file. </p>\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobOutputs\"\n        },\n        {\n          \"description\": \"<p>Information about the output files. We recommend that you use the <code>Outputs</code> syntax for all jobs, even\
  \ when you want Elastic Transcoder to transcode a file into only one format. Do not use both the <code>Outputs</code> and <code>Output</code> syntaxes in the same request. You can create a maximum of 30 outputs per job. </p> <p>If you specify more than one output for a job, Elastic Transcoder creates the files for each output in the order in which you specify them in the job.</p>\"\n        }\n      ]\n    },\n    \"OutputKeyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Key\"\n        },\n        {\n          \"description\": \"The value, if any, that you want Elastic Transcoder to prepend to the names of all files that this job creates, including output files, thumbnails, and playlists. We recommend that you add a / or some other delimiter to the end of the <code>OutputKeyPrefix</code>.\"\n        }\n      ]\n    },\n    \"Playlists\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Playlists\"\n        },\n       \
  \ {\n          \"description\": \"<important> <p>Outputs in Fragmented MP4 or MPEG-TS format only.</p> </important> <p>If you specify a preset in <code>PresetId</code> for which the value of <code>Container</code> is fmp4 (Fragmented MP4) or ts (MPEG-TS), <code>Playlists</code> contains information about the master playlists that you want Elastic Transcoder to create.</p> <p>The maximum number of master playlists in a job is 30.</p>\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \" The status of the job: <code>Submitted</code>, <code>Progressing</code>, <code>Complete</code>, <code>Canceled</code>, or <code>Error</code>. \"\n        }\n      ]\n    },\n    \"UserMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserMetadata\"\n        },\n        {\n          \"description\": \"<p>User-defined metadata that you\
  \ want to associate with an Elastic Transcoder job. You specify metadata in <code>key/value</code> pairs, and you can add up to 10 <code>key/value</code> pairs per job. Elastic Transcoder does not guarantee that <code>key/value</code> pairs are returned in the same order in which you specify them.</p> <p>Metadata <code>keys</code> and <code>values</code> must use characters from the following list:</p> <ul> <li> <p> <code>0-9</code> </p> </li> <li> <p> <code>A-Z</code> and <code>a-z</code> </p> </li> <li> <p> <code>Space</code> </p> </li> <li> <p>The following symbols: <code>_.:/=+-%@</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Timing\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timing\"\n        },\n        {\n          \"description\": \"Details about the timing of a job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-job-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: Job
---
