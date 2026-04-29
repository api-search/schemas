---
description: A Position object returned by the Apache Cordova Geolocation plugin containing coordinates and timestamp.
layout: schema
name: Position
properties_list:
- description: A set of geographic coordinates.
  name: coords
  type: object
- description: Creation time for coords as a DOMTimeStamp (milliseconds since UNIX epoch).
  name: timestamp
  type: integer
provider_name: Apache Cordova
provider_slug: apache-cordova
schema_file: json-schema/apache-cordova-geolocation-position-schema.json
slug: apache-cordova-geolocation-position
source_filename: apache-cordova-geolocation-position-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cordova/refs/heads/main/json-schema/apache-cordova-geolocation-position-schema.json\",\n  \"title\": \"Position\",\n  \"description\": \"A Position object returned by the Apache Cordova Geolocation plugin containing coordinates and timestamp.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"coords\": {\n      \"type\": \"object\",\n      \"description\": \"A set of geographic coordinates.\",\n      \"$id\": \"#Coordinates\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"Latitude in decimal degrees.\",\n          \"example\": 37.7749\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"Longitude in decimal degrees.\",\n          \"example\": -122.4194\n        },\n        \"altitude\": {\n          \"type\": \"number\"\
  ,\n          \"description\": \"Height of the position in meters above the ellipsoid.\",\n          \"example\": 15.0\n        },\n        \"accuracy\": {\n          \"type\": \"number\",\n          \"description\": \"Accuracy level of the latitude and longitude coordinates in meters.\",\n          \"example\": 10.0\n        },\n        \"altitudeAccuracy\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Accuracy level of the altitude coordinate in meters. null if not available.\",\n          \"example\": 5.0\n        },\n        \"heading\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Direction of travel, specified in degrees counting clockwise relative to true north. null if not available.\",\n          \"example\": 180.0\n        },\n        \"speed\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Current ground speed of the device, specified in meters per second. null if not available.\",\n\
  \          \"example\": 1.5\n        }\n      },\n      \"required\": [\"latitude\", \"longitude\", \"accuracy\"]\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation time for coords as a DOMTimeStamp (milliseconds since UNIX epoch).\",\n      \"example\": 1718153645993\n    }\n  },\n  \"required\": [\"coords\", \"timestamp\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cordova/refs/heads/main/json-schema/apache-cordova-geolocation-position-schema.json
tags:
- Apache
- Cross-Platform
- Hybrid Apps
- JavaScript
- Mobile
- Open Source
- Plugins
title: Position
---
