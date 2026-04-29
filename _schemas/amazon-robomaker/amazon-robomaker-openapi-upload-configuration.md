---
description: Provides upload configuration information. Files are uploaded from the simulation job to a location you specify.
layout: schema
name: UploadConfiguration
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: path
  type: object
- description: ''
  name: uploadBehavior
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-upload-configuration-schema.json
slug: amazon-robomaker-openapi-upload-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-upload-configuration-schema.json\",\n  \"title\": \"UploadConfiguration\",\n  \"description\": \"Provides upload configuration information. Files are uploaded from the simulation job to a location you specify. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>A prefix that specifies where files will be uploaded in Amazon S3. It is appended to the simulation output location to determine the final path. </p> <p> For example, if your simulation output location is <code>s3://my-bucket</code> and your upload configuration name is <code>robot-test</code>, your files will be uploaded to <code>s3://my-bucket/&lt;simid&gt;/&lt;runid&gt;/robot-test</code>.\
  \ </p>\"\n        }\n      ]\n    },\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Path\"\n        },\n        {\n          \"description\": \" Specifies the path of the file(s) to upload. Standard Unix glob matching rules are accepted, with the addition of <code>**</code> as a <i>super asterisk</i>. For example, specifying <code>/var/log/**.log</code> causes all .log files in the <code>/var/log</code> directory tree to be collected. For more examples, see <a href=\\\"https://github.com/gobwas/glob\\\">Glob Library</a>. \"\n        }\n      ]\n    },\n    \"uploadBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UploadBehavior\"\n        },\n        {\n          \"description\": \"<p>Specifies when to upload the files:</p> <dl> <dt>UPLOAD_ON_TERMINATE</dt> <dd> <p>Matching files are uploaded once the simulation enters the <code>TERMINATING</code> state. Matching files are not uploaded until all of your\
  \ code (including tools) have stopped. </p> <p>If there is a problem uploading a file, the upload is retried. If problems persist, no further upload attempts will be made.</p> </dd> <dt>UPLOAD_ROLLING_AUTO_REMOVE</dt> <dd> <p>Matching files are uploaded as they are created. They are deleted after they are uploaded. The specified path is checked every 5 seconds. A final check is made when all of your code (including tools) have stopped. </p> </dd> </dl>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"path\",\n    \"uploadBehavior\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-upload-configuration-schema.json
tags:
- AWS
- Robotics
- Simulation
title: UploadConfiguration
---
