---
description: Represents information about the remote access session.
layout: schema
name: RemoteAccessSession
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
  name: status
  type: object
- description: ''
  name: result
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: started
  type: object
- description: ''
  name: stopped
  type: object
- description: ''
  name: device
  type: object
- description: ''
  name: instanceArn
  type: object
- description: ''
  name: remoteDebugEnabled
  type: object
- description: ''
  name: remoteRecordEnabled
  type: object
- description: ''
  name: remoteRecordAppArn
  type: object
- description: ''
  name: hostAddress
  type: object
- description: ''
  name: clientId
  type: object
- description: ''
  name: billingMethod
  type: object
- description: ''
  name: deviceMinutes
  type: object
- description: ''
  name: endpoint
  type: object
- description: ''
  name: deviceUdid
  type: object
- description: ''
  name: interactionMode
  type: object
- description: ''
  name: skipAppResign
  type: object
- description: ''
  name: vpcConfig
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-remote-access-session-schema.json
slug: amazon-device-farm-remote-access-session
source_filename: amazon-device-farm-remote-access-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-remote-access-session-schema.json\",\n  \"title\": \"RemoteAccessSession\",\n  \"description\": \"Represents information about the remote access session.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the remote access session.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the remote access session.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n   \
  \     },\n        {\n          \"description\": \"The date and time the remote access session was created.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the remote access session. Can be any of the following:</p> <ul> <li> <p>PENDING.</p> </li> <li> <p>PENDING_CONCURRENCY.</p> </li> <li> <p>PENDING_DEVICE.</p> </li> <li> <p>PROCESSING.</p> </li> <li> <p>SCHEDULING.</p> </li> <li> <p>PREPARING.</p> </li> <li> <p>RUNNING.</p> </li> <li> <p>COMPLETED.</p> </li> <li> <p>STOPPING.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionResult\"\n        },\n        {\n          \"description\": \"<p>The result of the remote access session. Can be any of the following:</p> <ul> <li> <p>PENDING.</p> </li> <li> <p>PASSED.</p> </li> <li> <p>WARNED.</p>\
  \ </li> <li> <p>FAILED.</p> </li> <li> <p>SKIPPED.</p> </li> <li> <p>ERRORED.</p> </li> <li> <p>STOPPED.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"A message about the remote access session.\"\n        }\n      ]\n    },\n    \"started\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date and time the remote access session was started.\"\n        }\n      ]\n    },\n    \"stopped\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date and time the remote access session was stopped.\"\n        }\n      ]\n    },\n    \"device\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Device\"\n        },\n        {\n\
  \          \"description\": \"The device (phone or tablet) used in the remote access session.\"\n        }\n      ]\n    },\n    \"instanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the instance.\"\n        }\n      ]\n    },\n    \"remoteDebugEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>This flag is set to <code>true</code> if remote debugging is enabled for the remote access session.</p> <p>Remote debugging is <a href=\\\"https://docs.aws.amazon.com/devicefarm/latest/developerguide/history.html\\\">no longer supported</a>.</p>\"\n        }\n      ]\n    },\n    \"remoteRecordEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"This flag is set to <code>true</code>\
  \ if remote recording is enabled for the remote access session.\"\n        }\n      ]\n    },\n    \"remoteRecordAppArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN for the app to be recorded in the remote access session.\"\n        }\n      ]\n    },\n    \"hostAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HostAddress\"\n        },\n        {\n          \"description\": \"<p>IP address of the EC2 host where you need to connect to remotely debug devices. Only returned if remote debugging is enabled for the remote access session.</p> <p>Remote debugging is <a href=\\\"https://docs.aws.amazon.com/devicefarm/latest/developerguide/history.html\\\">no longer supported</a>.</p>\"\n        }\n      ]\n    },\n    \"clientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientId\"\n        },\n        {\n\
  \          \"description\": \"<p>Unique identifier of your client for the remote access session. Only returned if remote debugging is enabled for the remote access session.</p> <p>Remote debugging is <a href=\\\"https://docs.aws.amazon.com/devicefarm/latest/developerguide/history.html\\\">no longer supported</a>.</p>\"\n        }\n      ]\n    },\n    \"billingMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingMethod\"\n        },\n        {\n          \"description\": \"The billing method of the remote access session. Possible values include <code>METERED</code> or <code>UNMETERED</code>. For more information about metered devices, see <a href=\\\"https://docs.aws.amazon.com/devicefarm/latest/developerguide/welcome.html#welcome-terminology\\\">AWS Device Farm terminology</a>.\"\n        }\n      ]\n    },\n    \"deviceMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceMinutes\"\n        },\n        {\n\
  \          \"description\": \"The number of minutes a device is used in a remote access session (including setup and teardown minutes).\"\n        }\n      ]\n    },\n    \"endpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The endpoint for the remote access sesssion.\"\n        }\n      ]\n    },\n    \"deviceUdid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Unique device identifier for the remote device. Only returned if remote debugging is enabled for the remote access session.</p> <p>Remote debugging is <a href=\\\"https://docs.aws.amazon.com/devicefarm/latest/developerguide/history.html\\\">no longer supported</a>.</p>\"\n        }\n      ]\n    },\n    \"interactionMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InteractionMode\"\n        },\n   \
  \     {\n          \"description\": \"<p>The interaction mode of the remote access session. Valid values are:</p> <ul> <li> <p>INTERACTIVE: You can interact with the iOS device by viewing, touching, and rotating the screen. You cannot run XCUITest framework-based tests in this mode.</p> </li> <li> <p>NO_VIDEO: You are connected to the device, but cannot interact with it or view the screen. This mode has the fastest test execution speed. You can run XCUITest framework-based tests in this mode.</p> </li> <li> <p>VIDEO_ONLY: You can view the screen, but cannot touch or rotate it. You can run XCUITest framework-based tests and watch the screen in this mode.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"skipAppResign\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SkipAppResign\"\n        },\n        {\n          \"description\": \"<p>When set to <code>true</code>, for private devices, Device Farm does not sign your app again. For public devices, Device\
  \ Farm always signs your apps again.</p> <p>For more information about how Device Farm re-signs your apps, see <a href=\\\"http://aws.amazon.com/device-farm/faqs/\\\">Do you modify my app?</a> in the <i>AWS Device Farm FAQs</i>.</p>\"\n        }\n      ]\n    },\n    \"vpcConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfig\"\n        },\n        {\n          \"description\": \"The VPC security groups and subnets that are attached to a project.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-remote-access-session-schema.json
tags:
- Application Testing
- Device Testing
- Mobile Testing
- Quality Assurance
title: RemoteAccessSession
---
