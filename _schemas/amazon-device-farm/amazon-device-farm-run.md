---
description: Represents a test run on a set of devices with a given app package, test parameters, and so on.
layout: schema
name: Run
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: result
  type: object
- description: ''
  name: started
  type: object
- description: ''
  name: stopped
  type: object
- description: ''
  name: counters
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: totalJobs
  type: object
- description: ''
  name: completedJobs
  type: object
- description: ''
  name: billingMethod
  type: object
- description: ''
  name: deviceMinutes
  type: object
- description: ''
  name: networkProfile
  type: object
- description: ''
  name: parsingResultUrl
  type: object
- description: ''
  name: resultCode
  type: object
- description: ''
  name: seed
  type: object
- description: ''
  name: appUpload
  type: object
- description: ''
  name: eventCount
  type: object
- description: ''
  name: jobTimeoutMinutes
  type: object
- description: ''
  name: devicePoolArn
  type: object
- description: ''
  name: locale
  type: object
- description: ''
  name: radios
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: customerArtifactPaths
  type: object
- description: ''
  name: webUrl
  type: object
- description: ''
  name: skipAppResign
  type: object
- description: ''
  name: testSpecArn
  type: object
- description: ''
  name: deviceSelectionResult
  type: object
- description: ''
  name: vpcConfig
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-run-schema.json
slug: amazon-device-farm-run
source_filename: amazon-device-farm-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-run-schema.json\",\n  \"title\": \"Run\",\n  \"description\": \"Represents a test run on a set of devices with a given app package, test parameters, and so on.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The run's ARN.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The run's name.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TestType\"\n        },\n        {\n          \"description\": \"<p>The run's type.</p>\
  \ <p>Must be one of the following values:</p> <ul> <li> <p>BUILTIN_FUZZ</p> </li> <li> <p>BUILTIN_EXPLORER</p> <note> <p>For Android, an app explorer that traverses an Android app, interacting with it and capturing screenshots at the same time.</p> </note> </li> <li> <p>APPIUM_JAVA_JUNIT</p> </li> <li> <p>APPIUM_JAVA_TESTNG</p> </li> <li> <p>APPIUM_PYTHON</p> </li> <li> <p>APPIUM_NODE</p> </li> <li> <p>APPIUM_RUBY</p> </li> <li> <p>APPIUM_WEB_JAVA_JUNIT</p> </li> <li> <p>APPIUM_WEB_JAVA_TESTNG</p> </li> <li> <p>APPIUM_WEB_PYTHON</p> </li> <li> <p>APPIUM_WEB_NODE</p> </li> <li> <p>APPIUM_WEB_RUBY</p> </li> <li> <p>CALABASH</p> </li> <li> <p>INSTRUMENTATION</p> </li> <li> <p>UIAUTOMATION</p> </li> <li> <p>UIAUTOMATOR</p> </li> <li> <p>XCTEST</p> </li> <li> <p>XCTEST_UI</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevicePlatform\"\n        },\n        {\n          \"description\": \"<p>The run's\
  \ platform.</p> <p>Allowed values include:</p> <ul> <li> <p>ANDROID</p> </li> <li> <p>IOS</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"When the run was created.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionStatus\"\n        },\n        {\n          \"description\": \"<p>The run's status.</p> <p>Allowed values include:</p> <ul> <li> <p>PENDING</p> </li> <li> <p>PENDING_CONCURRENCY</p> </li> <li> <p>PENDING_DEVICE</p> </li> <li> <p>PROCESSING</p> </li> <li> <p>SCHEDULING</p> </li> <li> <p>PREPARING</p> </li> <li> <p>RUNNING</p> </li> <li> <p>COMPLETED</p> </li> <li> <p>STOPPING</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionResult\"\n        },\n\
  \        {\n          \"description\": \"<p>The run's result.</p> <p>Allowed values include:</p> <ul> <li> <p>PENDING</p> </li> <li> <p>PASSED</p> </li> <li> <p>WARNED</p> </li> <li> <p>FAILED</p> </li> <li> <p>SKIPPED</p> </li> <li> <p>ERRORED</p> </li> <li> <p>STOPPED</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"started\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The run's start time.\"\n        }\n      ]\n    },\n    \"stopped\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The run's stop time.\"\n        }\n      ]\n    },\n    \"counters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Counters\"\n        },\n        {\n          \"description\": \"The run's result counters.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"A message about the run's result.\"\n        }\n      ]\n    },\n    \"totalJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of jobs for the run.\"\n        }\n      ]\n    },\n    \"completedJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of completed jobs.\"\n        }\n      ]\n    },\n    \"billingMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingMethod\"\n        },\n        {\n          \"description\": \"<p>Specifies the billing method for a test run: <code>metered</code> or <code>unmetered</code>. If the parameter is not specified, the default value is <code>metered</code>.</p> <note> <p>If you\
  \ have unmetered device slots, you must set this to <code>unmetered</code> to use them. Otherwise, the run is counted toward metered device minutes.</p> </note>\"\n        }\n      ]\n    },\n    \"deviceMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceMinutes\"\n        },\n        {\n          \"description\": \"Represents the total (metered or unmetered) minutes used by the test run.\"\n        }\n      ]\n    },\n    \"networkProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkProfile\"\n        },\n        {\n          \"description\": \"The network profile being used for a test run.\"\n        }\n      ]\n    },\n    \"parsingResultUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Read-only URL for an object in an S3 bucket where you can get the parsing results of the test package. If the test package\
  \ doesn't parse, the reason why it doesn't parse appears in the file that this URL points to.\"\n        }\n      ]\n    },\n    \"resultCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionResultCode\"\n        },\n        {\n          \"description\": \"Supporting field for the result field. Set only if <code>result</code> is <code>SKIPPED</code>. <code>PARSING_FAILED</code> if the result is skipped because of test package parsing failure.\"\n        }\n      ]\n    },\n    \"seed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"For fuzz tests, this is a seed to use for randomizing the UI fuzz test. Using the same seed value between tests ensures identical event sequences.\"\n        }\n      ]\n    },\n    \"appUpload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n        \
  \  \"description\": \"An app to upload or that has been uploaded.\"\n        }\n      ]\n    },\n    \"eventCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"For fuzz tests, this is the number of events, between 1 and 10000, that the UI fuzz test should perform.\"\n        }\n      ]\n    },\n    \"jobTimeoutMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTimeoutMinutes\"\n        },\n        {\n          \"description\": \"The number of minutes the job executes before it times out.\"\n        }\n      ]\n    },\n    \"devicePoolArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the device pool for the run.\"\n        }\n      ]\n    },\n    \"locale\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"Information about the locale that is used for the run.\"\n        }\n      ]\n    },\n    \"radios\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Radios\"\n        },\n        {\n          \"description\": \"Information about the radio states for the run.\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Location\"\n        },\n        {\n          \"description\": \"Information about the location that is used for the run.\"\n        }\n      ]\n    },\n    \"customerArtifactPaths\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerArtifactPaths\"\n        },\n        {\n          \"description\": \"Output <code>CustomerArtifactPaths</code> object for the test run.\"\n        }\n      ]\n    },\n    \"webUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The Device Farm console URL for the recording of the run.\"\n        }\n      ]\n    },\n    \"skipAppResign\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SkipAppResign\"\n        },\n        {\n          \"description\": \"<p>When set to <code>true</code>, for private devices, Device Farm does not sign your app again. For public devices, Device Farm always signs your apps again.</p> <p>For more information about how Device Farm re-signs your apps, see <a href=\\\"http://aws.amazon.com/device-farm/faqs/\\\">Do you modify my app?</a> in the <i>AWS Device Farm FAQs</i>.</p>\"\n        }\n      ]\n    },\n    \"testSpecArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the YAML-formatted test specification for the run.\"\n        }\n      ]\n    },\n    \"deviceSelectionResult\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceSelectionResult\"\n        },\n        {\n          \"description\": \"The results of a device filter used to select the devices for a test run.\"\n        }\n      ]\n    },\n    \"vpcConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfig\"\n        },\n        {\n          \"description\": \"The VPC security groups and subnets that are attached to a project.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-run-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: Run
---
