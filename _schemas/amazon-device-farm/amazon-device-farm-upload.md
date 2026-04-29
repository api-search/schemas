---
description: An app or a set of one or more tests to upload or that have been uploaded.
layout: schema
name: Upload
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: url
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: contentType
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: category
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-upload-schema.json
slug: amazon-device-farm-upload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-upload-schema.json\",\n  \"title\": \"Upload\",\n  \"description\": \"An app or a set of one or more tests to upload or that have been uploaded.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The upload's ARN.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The upload's file name.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"When the upload was\
  \ created.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UploadType\"\n        },\n        {\n          \"description\": \"<p>The upload's type.</p> <p>Must be one of the following values:</p> <ul> <li> <p>ANDROID_APP</p> </li> <li> <p>IOS_APP</p> </li> <li> <p>WEB_APP</p> </li> <li> <p>EXTERNAL_DATA</p> </li> <li> <p>APPIUM_JAVA_JUNIT_TEST_PACKAGE</p> </li> <li> <p>APPIUM_JAVA_TESTNG_TEST_PACKAGE</p> </li> <li> <p>APPIUM_PYTHON_TEST_PACKAGE</p> </li> <li> <p>APPIUM_NODE_TEST_PACKAGE</p> </li> <li> <p>APPIUM_RUBY_TEST_PACKAGE</p> </li> <li> <p>APPIUM_WEB_JAVA_JUNIT_TEST_PACKAGE</p> </li> <li> <p>APPIUM_WEB_JAVA_TESTNG_TEST_PACKAGE</p> </li> <li> <p>APPIUM_WEB_PYTHON_TEST_PACKAGE</p> </li> <li> <p>APPIUM_WEB_NODE_TEST_PACKAGE</p> </li> <li> <p>APPIUM_WEB_RUBY_TEST_PACKAGE</p> </li> <li> <p>CALABASH_TEST_PACKAGE</p> </li> <li> <p>INSTRUMENTATION_TEST_PACKAGE</p> </li> <li> <p>UIAUTOMATION_TEST_PACKAGE</p> </li> <li>\
  \ <p>UIAUTOMATOR_TEST_PACKAGE</p> </li> <li> <p>XCTEST_TEST_PACKAGE</p> </li> <li> <p>XCTEST_UI_TEST_PACKAGE</p> </li> <li> <p>APPIUM_JAVA_JUNIT_TEST_SPEC</p> </li> <li> <p>APPIUM_JAVA_TESTNG_TEST_SPEC</p> </li> <li> <p>APPIUM_PYTHON_TEST_SPEC</p> </li> <li> <p>APPIUM_NODE_TEST_SPEC</p> </li> <li> <p>APPIUM_RUBY_TEST_SPEC</p> </li> <li> <p>APPIUM_WEB_JAVA_JUNIT_TEST_SPEC</p> </li> <li> <p>APPIUM_WEB_JAVA_TESTNG_TEST_SPEC</p> </li> <li> <p>APPIUM_WEB_PYTHON_TEST_SPEC</p> </li> <li> <p>APPIUM_WEB_NODE_TEST_SPEC</p> </li> <li> <p>APPIUM_WEB_RUBY_TEST_SPEC</p> </li> <li> <p>INSTRUMENTATION_TEST_SPEC</p> </li> <li> <p>XCTEST_UI_TEST_SPEC</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UploadStatus\"\n        },\n        {\n          \"description\": \"<p>The upload's status.</p> <p>Must be one of the following values:</p> <ul> <li> <p>FAILED</p> </li> <li> <p>INITIALIZED</p> </li> <li> <p>PROCESSING</p>\
  \ </li> <li> <p>SUCCEEDED</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveURL\"\n        },\n        {\n          \"description\": \"The presigned Amazon S3 URL that was used to store a file using a PUT request.\"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Metadata\"\n        },\n        {\n          \"description\": \"The upload's metadata. For example, for Android, this contains information that is parsed from the manifest and is displayed in the AWS Device Farm console after the associated app is uploaded.\"\n        }\n      ]\n    },\n    \"contentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContentType\"\n        },\n        {\n          \"description\": \"The upload's content type (for example, <code>application/octet-stream</code>).\"\n        }\n      ]\n    },\n\
  \    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"A message about the upload's result.\"\n        }\n      ]\n    },\n    \"category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UploadCategory\"\n        },\n        {\n          \"description\": \"<p>The upload's category. Allowed values include:</p> <ul> <li> <p>CURATED: An upload managed by AWS Device Farm.</p> </li> <li> <p>PRIVATE: An upload managed by the AWS Device Farm customer.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-upload-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: Upload
---
