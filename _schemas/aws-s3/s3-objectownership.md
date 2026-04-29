---
description: <p>The container element for object ownership for a bucket's ownership controls.</p> <p>BucketOwnerPreferred - Objects uploaded to the bucket change ownership to the bucket owner if the objects are uploaded with the <code>bucket-owner-full-control</code> canned ACL.</p> <p>ObjectWriter - The uploading account will own the object if the object is uploaded with the <code>bucket-owner-full-control</code> canned ACL.</p> <p>BucketOwnerEnforced - Access control lists (ACLs) are disabled and no longer affect permissions. The bucket owner automatically owns and has full control over every object in the bucket. The bucket only accepts PUT requests that don't specify an ACL or bucket owner full control ACLs, such as the <code>bucket-owner-full-control</code> canned ACL or an equivalent form of this ACL expressed in the XML format.</p>
layout: schema
name: ObjectOwnership
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectownership-schema.json
slug: s3-objectownership
source_filename: s3-objectownership-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectOwnership\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"BucketOwnerPreferred\",\n    \"ObjectWriter\",\n    \"BucketOwnerEnforced\"\n  ],\n  \"description\": \"<p>The container element for object ownership for a bucket's ownership controls.</p> <p>BucketOwnerPreferred - Objects uploaded to the bucket change ownership to the bucket owner if the objects are uploaded with the <code>bucket-owner-full-control</code> canned ACL.</p> <p>ObjectWriter - The uploading account will own the object if the object is uploaded with the <code>bucket-owner-full-control</code> canned ACL.</p> <p>BucketOwnerEnforced - Access control lists (ACLs) are disabled and no longer affect permissions. The bucket owner automatically owns and has full control over every object in the bucket. The bucket only accepts PUT requests that don't specify an ACL or bucket owner full control ACLs, such as the <code>bucket-owner-full-control</code>\
  \ canned ACL or an equivalent form of this ACL expressed in the XML format.</p>\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectownership-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ObjectOwnership
---
