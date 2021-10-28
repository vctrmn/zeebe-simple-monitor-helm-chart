# Zeebe Simple Monitor Helm Chart for Hazelcast

Helm chart for simple monitor, the monitoring application for [Zeebe](https://zeebe.io). It is designed for developers to
* get in touch with Zeebe and workflow execution (BPMN)
* test workflows manually
* provide insides on how workflows are executed 

## Requirements

* [Helm](https://helm.sh/) >= 3.x +
* Kubernetes >= 1.18
* Hazelcast deployed
* Zeebe 1.x deployed
* Minimum cluster requirements include the following to run this chart with default settings. All of these settings are configurable.
  * 1GB of RAM for the JVM heap

 ## Configuration
  | Parameter                     | Description                                                                                                                                                                                                                                                                                                                | Default                                                                                                                   |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| `global.hazelcast.host`   | Hazelcast host to use in Hazelcast Exporter connection  | `hazelcast` |
| `global.hazelcast.port`   | Hazelcast port to use in Hazelcast Exporter connection | `5701` |
| `global.zeebe.host`       | Zeebe broker host contact point | `zeebe-gateway` |
| `global.zeebe.host`       | Zeebe broker port contact point | `26500` |                                                                                                                                                                        

