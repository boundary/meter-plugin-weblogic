# TrueSight Pulse WebLogic Plugin

Uses JMX protocol to collect measurements from 1 or more instances of WebLogic that is ethier co-resident with the meter the plugin is running on or remotely.

### Prerequisites

|     OS    | Linux | Windows | SmartOS | OS X |
|:----------|:-----:|:-------:|:-------:|:----:|
| Supported |   v   |    v    |    v    |  v   |

* Java 1.7 or later.
* This plugin is compatible with WebLogic X.X.X or later.

#### Boundary Meter versions v4.2 or later

- To install new meter go to Settings->Installation or [see instructions](https://help.boundary.com/hc/en-us/sections/200634331-Installation).
- To upgrade the meter to the latest version - [see instructions](https://help.boundary.com/hc/en-us/articles/201573102-Upgrading-the-Boundary-Meter).

### Plugin Setup

To collect statistics from a WebLogic instance you need to enable access to the JMX remote endpoint.

```
$ # Specific commands and instructions to be determined

```

### Plugin Configuration Fields

|Field Name     | Description                                                                                |
|:--------------|:-------------------------------------------------------------------------------------------|
| Host          | Host of the WebLogic JMX endpoint.                                                         |
| Port          | Port of the WebLogic JMX endpoint. Defaults to XXXX.                                       |
| Username      | Username of the WebLogic JMX endpoint.                                                     |
| Password      | Password of the WebLogic JMX endpoint.                                                     |
| Source        | The Source to display in the legend for the metrics data (default: hostname of the server).|
| Poll Interval | How often should the plugin poll for metrics. |

### Metrics Collected

|Metric Name                   |Description                                                               |
|:-----------------------------|:----------------------------------------------|
| WEBLOGIC_JVM_HEAPMEMORY_USED | Heap memory used by the java virtual machine. |

### Dashboards

- WebLogic

### References

[https://docs.oracle.com/cd/E13222_01/wls/docs90/jmx/accessWLS.html](https://docs.oracle.com/cd/E13222_01/wls/docs90/jmx/accessWLS.html)
