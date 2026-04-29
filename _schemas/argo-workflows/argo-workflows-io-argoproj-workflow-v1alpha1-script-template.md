---
description: ScriptTemplate is a template subtype to enable scripting through code steps
layout: schema
name: io.argoproj.workflow.v1alpha1.ScriptTemplate
properties_list:
- description: Arguments to the entrypoint. The container image's CMD is used if this is not provided. Variable references $(VAR_NAME) are expanded using the container's environment. If a variable cannot be resolved
  name: args
  type: array
- description: Entrypoint array. Not executed within a shell. The container image's ENTRYPOINT is used if this is not provided. Variable references $(VAR_NAME) are expanded using the container's environment. If a va
  name: command
  type: array
- description: List of environment variables to set in the container. Cannot be updated.
  name: env
  type: array
- description: List of sources to populate environment variables in the container. The keys defined within a source may consist of any printable ASCII characters except '='. When a key exists in multiple sources, th
  name: envFrom
  type: array
- description: 'Container image name. More info: https://kubernetes.io/docs/concepts/containers/images This field is optional to allow higher level config management to default or override container images in workloa'
  name: image
  type: string
- description: 'Image pull policy. One of Always, Never, IfNotPresent. Defaults to Always if :latest tag is specified, or IfNotPresent otherwise. Cannot be updated. More info: https://kubernetes.io/docs/concepts/cont'
  name: imagePullPolicy
  type: string
- description: Actions that the management system should take in response to container lifecycle events. Cannot be updated.
  name: lifecycle
  type: object
- description: 'Periodic probe of container liveness. Container will be restarted if the probe fails. Cannot be updated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes'
  name: livenessProbe
  type: object
- description: Name of the container specified as a DNS_LABEL. Each container in a pod must have a unique name (DNS_LABEL). Cannot be updated.
  name: name
  type: string
- description: List of ports to expose from the container. Not specifying a port here DOES NOT prevent that port from being exposed. Any port which is listening on the default "0.0.0.0" address inside a container wi
  name: ports
  type: array
- description: 'Periodic probe of container service readiness. Container will be removed from service endpoints if the probe fails. Cannot be updated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod'
  name: readinessProbe
  type: object
- description: Resources resize policy for the container. This field cannot be set on ephemeral containers.
  name: resizePolicy
  type: array
- description: 'Compute Resources required by this container. Cannot be updated. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/'
  name: resources
  type: object
- description: RestartPolicy defines the restart behavior of individual containers in a pod. This overrides the pod-level restart policy. When this field is not specified, the restart behavior is defined by the Pod'
  name: restartPolicy
  type: string
- description: Represents a list of rules to be checked to determine if the container should be restarted on exit. The rules are evaluated in order. Once a rule matches a container exit condition, the remaining rule
  name: restartPolicyRules
  type: array
- description: 'SecurityContext defines the security options the container should be run with. If set, the fields of SecurityContext override the equivalent fields of PodSecurityContext. More info: https://kubernetes'
  name: securityContext
  type: object
- description: Source contains the source code of the script to execute
  name: source
  type: string
- description: 'StartupProbe indicates that the Pod has successfully initialized. If specified, no other probes are executed until this completes successfully. If this probe fails, the Pod will be restarted, just as '
  name: startupProbe
  type: object
- description: Whether this container should allocate a buffer for stdin in the container runtime. If this is not set, reads from stdin in the container will always result in EOF. Default is false.
  name: stdin
  type: boolean
- description: Whether the container runtime should close the stdin channel after it has been opened by a single attach. When stdin is true the stdin stream will remain open across multiple attach sessions. If stdin
  name: stdinOnce
  type: boolean
- description: 'Optional: Path at which the file to which the container''s termination message will be written is mounted into the container''s filesystem. Message written is intended to be brief final status, such as '
  name: terminationMessagePath
  type: string
- description: Indicate how the termination message should be populated. File will use the contents of terminationMessagePath to populate the container status message on both success and failure. FallbackToLogsOnErr
  name: terminationMessagePolicy
  type: string
- description: Whether this container should allocate a TTY for itself, also requires 'stdin' to be true. Default is false.
  name: tty
  type: boolean
- description: volumeDevices is the list of block devices to be used by the container.
  name: volumeDevices
  type: array
- description: Pod volumes to mount into the container's filesystem. Cannot be updated.
  name: volumeMounts
  type: array
- description: Container's working directory. If not specified, the container runtime's default will be used, which might be configured in the container image. Cannot be updated.
  name: workingDir
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-script-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-script-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-script-template-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ScriptTemplate\",\n  \"description\": \"ScriptTemplate is a template subtype to enable scripting through code steps\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"args\": {\n      \"description\": \"Arguments to the entrypoint. The container image's CMD is used if this is not provided. Variable references $(VAR_NAME) are expanded using the container's environment. If a variable cannot be resolved, the reference in the input string will be unchanged. Double $$ are reduced to a single $, which allows for escaping the $(VAR_NAME) syntax: i.e. \\\"$$(VAR_NAME)\\\" will produce the string literal \\\"$(VAR_NAME)\\\". Escaped references will never be expanded, regardless of whether\
  \ the variable exists or not. Cannot be updated. More info: https://kubernetes.io/docs/tasks/inject-data-application/define-command-argument-container/#running-a-command-in-a-shell\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"command\": {\n      \"description\": \"Entrypoint array. Not executed within a shell. The container image's ENTRYPOINT is used if this is not provided. Variable references $(VAR_NAME) are expanded using the container's environment. If a variable cannot be resolved, the reference in the input string will be unchanged. Double $$ are reduced to a single $, which allows for escaping the $(VAR_NAME) syntax: i.e. \\\"$$(VAR_NAME)\\\" will produce the string literal \\\"$(VAR_NAME)\\\". Escaped references will never be expanded, regardless of whether the variable exists or not. Cannot be updated. More info: https://kubernetes.io/docs/tasks/inject-data-application/define-command-argument-container/#running-a-command-in-a-shell\"\
  ,\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"env\": {\n      \"description\": \"List of environment variables to set in the container. Cannot be updated.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.EnvVar\"\n      },\n      \"x-kubernetes-list-map-keys\": [\n        \"name\"\n      ],\n      \"x-kubernetes-list-type\": \"map\",\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"envFrom\": {\n      \"description\": \"List of sources to populate environment variables in the container. The keys defined within a source may consist of any printable ASCII characters except '='. When a key exists in multiple sources, the value associated with the last source will take precedence. Values defined by an Env with a duplicate key will take precedence. Cannot be updated.\"\
  ,\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.EnvFromSource\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"image\": {\n      \"description\": \"Container image name. More info: https://kubernetes.io/docs/concepts/containers/images This field is optional to allow higher level config management to default or override container images in workload controllers like Deployments and StatefulSets.\",\n      \"type\": \"string\"\n    },\n    \"imagePullPolicy\": {\n      \"description\": \"Image pull policy. One of Always, Never, IfNotPresent. Defaults to Always if :latest tag is specified, or IfNotPresent otherwise. Cannot be updated. More info: https://kubernetes.io/docs/concepts/containers/images#updating-images\",\n      \"type\": \"string\"\n    },\n    \"lifecycle\": {\n      \"description\": \"Actions that the management system should take in response to container lifecycle events. Cannot be updated.\",\n\
  \      \"$ref\": \"#/definitions/io.k8s.api.core.v1.Lifecycle\"\n    },\n    \"livenessProbe\": {\n      \"description\": \"Periodic probe of container liveness. Container will be restarted if the probe fails. Cannot be updated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.Probe\"\n    },\n    \"name\": {\n      \"description\": \"Name of the container specified as a DNS_LABEL. Each container in a pod must have a unique name (DNS_LABEL). Cannot be updated.\",\n      \"type\": \"string\"\n    },\n    \"ports\": {\n      \"description\": \"List of ports to expose from the container. Not specifying a port here DOES NOT prevent that port from being exposed. Any port which is listening on the default \\\"0.0.0.0\\\" address inside a container will be accessible from the network. Modifying this array with strategic merge patch may corrupt the data. For more information See https://github.com/kubernetes/kubernetes/issues/108255.\
  \ Cannot be updated.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.ContainerPort\"\n      },\n      \"x-kubernetes-list-map-keys\": [\n        \"containerPort\",\n        \"protocol\"\n      ],\n      \"x-kubernetes-list-type\": \"map\",\n      \"x-kubernetes-patch-merge-key\": \"containerPort\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"readinessProbe\": {\n      \"description\": \"Periodic probe of container service readiness. Container will be removed from service endpoints if the probe fails. Cannot be updated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.Probe\"\n    },\n    \"resizePolicy\": {\n      \"description\": \"Resources resize policy for the container. This field cannot be set on ephemeral containers.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.ContainerResizePolicy\"\
  \n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"resources\": {\n      \"description\": \"Compute Resources required by this container. Cannot be updated. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ResourceRequirements\"\n    },\n    \"restartPolicy\": {\n      \"description\": \"RestartPolicy defines the restart behavior of individual containers in a pod. This overrides the pod-level restart policy. When this field is not specified, the restart behavior is defined by the Pod's restart policy and the container type. Additionally, setting the RestartPolicy as \\\"Always\\\" for the init container will have the following effect: this init container will be continually restarted on exit until all regular containers have terminated. Once all regular containers have completed, all init containers with restartPolicy \\\"Always\\\" will be shut down. This lifecycle differs\
  \ from normal init containers and is often referred to as a \\\"sidecar\\\" container. Although this init container still starts in the init container sequence, it does not wait for the container to complete before proceeding to the next init container. Instead, the next init container starts immediately after this init container is started, or after any startupProbe has successfully completed.\",\n      \"type\": \"string\"\n    },\n    \"restartPolicyRules\": {\n      \"description\": \"Represents a list of rules to be checked to determine if the container should be restarted on exit. The rules are evaluated in order. Once a rule matches a container exit condition, the remaining rules are ignored. If no rule matches the container exit condition, the Container-level restart policy determines the whether the container is restarted or not. Constraints on the rules: - At most 20 rules are allowed. - Rules can have the same action. - Identical rules are not forbidden in validations. When\
  \ rules are specified, container MUST set RestartPolicy explicitly even it if matches the Pod's RestartPolicy.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.ContainerRestartRule\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"securityContext\": {\n      \"description\": \"SecurityContext defines the security options the container should be run with. If set, the fields of SecurityContext override the equivalent fields of PodSecurityContext. More info: https://kubernetes.io/docs/tasks/configure-pod-container/security-context/\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecurityContext\"\n    },\n    \"source\": {\n      \"description\": \"Source contains the source code of the script to execute\",\n      \"type\": \"string\"\n    },\n    \"startupProbe\": {\n      \"description\": \"StartupProbe indicates that the Pod has successfully initialized. If specified, no other probes are executed until\
  \ this completes successfully. If this probe fails, the Pod will be restarted, just as if the livenessProbe failed. This can be used to provide different probe parameters at the beginning of a Pod's lifecycle, when it might take a long time to load data or warm a cache, than during steady-state operation. This cannot be updated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.Probe\"\n    },\n    \"stdin\": {\n      \"description\": \"Whether this container should allocate a buffer for stdin in the container runtime. If this is not set, reads from stdin in the container will always result in EOF. Default is false.\",\n      \"type\": \"boolean\"\n    },\n    \"stdinOnce\": {\n      \"description\": \"Whether the container runtime should close the stdin channel after it has been opened by a single attach. When stdin is true the stdin stream will remain open across multiple attach sessions.\
  \ If stdinOnce is set to true, stdin is opened on container start, is empty until the first client attaches to stdin, and then remains open and accepts data until the client disconnects, at which time stdin is closed and remains closed until the container is restarted. If this flag is false, a container processes that reads from stdin will never receive an EOF. Default is false\",\n      \"type\": \"boolean\"\n    },\n    \"terminationMessagePath\": {\n      \"description\": \"Optional: Path at which the file to which the container's termination message will be written is mounted into the container's filesystem. Message written is intended to be brief final status, such as an assertion failure message. Will be truncated by the node if greater than 4096 bytes. The total message length across all containers will be limited to 12kb. Defaults to /dev/termination-log. Cannot be updated.\",\n      \"type\": \"string\"\n    },\n    \"terminationMessagePolicy\": {\n      \"description\": \"Indicate\
  \ how the termination message should be populated. File will use the contents of terminationMessagePath to populate the container status message on both success and failure. FallbackToLogsOnError will use the last chunk of container log output if the termination message file is empty and the container exited with an error. The log output is limited to 2048 bytes or 80 lines, whichever is smaller. Defaults to File. Cannot be updated.\",\n      \"type\": \"string\"\n    },\n    \"tty\": {\n      \"description\": \"Whether this container should allocate a TTY for itself, also requires 'stdin' to be true. Default is false.\",\n      \"type\": \"boolean\"\n    },\n    \"volumeDevices\": {\n      \"description\": \"volumeDevices is the list of block devices to be used by the container.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.VolumeDevice\"\n      },\n      \"x-kubernetes-list-map-keys\": [\n        \"devicePath\"\n      ],\n  \
  \    \"x-kubernetes-list-type\": \"map\",\n      \"x-kubernetes-patch-merge-key\": \"devicePath\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"volumeMounts\": {\n      \"description\": \"Pod volumes to mount into the container's filesystem. Cannot be updated.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.VolumeMount\"\n      },\n      \"x-kubernetes-list-map-keys\": [\n        \"mountPath\"\n      ],\n      \"x-kubernetes-list-type\": \"map\",\n      \"x-kubernetes-patch-merge-key\": \"mountPath\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"workingDir\": {\n      \"description\": \"Container's working directory. If not specified, the container runtime's default will be used, which might be configured in the container image. Cannot be updated.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"image\",\n    \"source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-script-template-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ScriptTemplate
---
