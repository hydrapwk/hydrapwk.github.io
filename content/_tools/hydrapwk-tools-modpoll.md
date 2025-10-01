---
layout: tools-doc
title: modpoll
permalink: /doc/tools/hydrapwk-tools-modpoll
comments: true
tool-icons: /assets/graphics/tools_graphics/hydrapwk-icons-missing.svg
tool-version: blank
packages-name: modpoll
tools-command: modpoll --help
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: M
update: 2025-09-30 06:02:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-modpoll.md
---

```
Modpoll v1.5.0 - A New Command-line Tool for Modbus and MQTT

usage: modpoll [-h] [-v] -f CONFIG [CONFIG ...] [-d] [-r RATE] [-1]
               [--interval INTERVAL] [--tcp TCP] [--tcp-port TCP_PORT]
               [--udp UDP] [--udp-port UDP_PORT] [--rtu RTU]
               [--rtu-baud RTU_BAUD] [--rtu-parity {none,odd,even}]
               [--timeout TIMEOUT] [-o EXPORT] [--mqtt-version {3.1.1,5.0}]
               [--mqtt-host MQTT_HOST] [--mqtt-port MQTT_PORT]
               [--mqtt-clientid MQTT_CLIENTID]
               [--mqtt-topic-prefix MQTT_TOPIC_PREFIX]
               [--mqtt-publish-topic-pattern MQTT_PUBLISH_TOPIC_PATTERN]
               [--mqtt-subscribe-topic-pattern MQTT_SUBSCRIBE_TOPIC_PATTERN]
               [--mqtt-diagnostics-topic-pattern MQTT_DIAGNOSTICS_TOPIC_PATTERN]
               [--mqtt-qos {0,1,2}] [--mqtt-user MQTT_USER]
               [--mqtt-pass MQTT_PASS] [--mqtt-use-tls] [--mqtt-insecure]
               [--mqtt-cacerts MQTT_CACERTS]
               [--mqtt-tls-version {tlsv1.2,tlsv1.1,tlsv1}] [--mqtt-single]
               [--diagnostics-rate DIAGNOSTICS_RATE] [--autoremove]
               [--loglevel {DEBUG,INFO,WARNING,ERROR,CRITICAL}] [--timestamp]
               [--delay DELAY] [--framer {default,ascii,binary,rtu,socket}]

Modpoll v1.5.0 - A New Command-line Tool for Modbus and MQTT

options:
  -h, --help            show this help message and exit
  -v, --version         show program's version number and exit
  -f, --config CONFIG [CONFIG ...]
                        A local path or URL of Modbus configuration file.
                        Required!
  -d, --daemon          Run in daemon mode without printing result.
                        Recommended to use with docker
  -r, --rate RATE       The sampling rate (s) to poll modbus device, Defaults
                        to 10.0
  -1, --once            Only run polling at one time
  --interval INTERVAL   The time interval in seconds between two polling,
                        Defaults to 0.5
  --tcp TCP             Act as a Modbus TCP master, connecting to host TCP
  --tcp-port TCP_PORT   Port for MODBUS TCP. Defaults to 502
  --udp UDP             Act as a Modbus UDP master, connecting to host UDP
  --udp-port UDP_PORT   Port for MODBUS UDP. Defaults to 502
  --rtu RTU             pyserial URL (or port name) for RTU serial port
  --rtu-baud RTU_BAUD   Baud rate for serial port. Defaults to 9600
  --rtu-parity {none,odd,even}
                        Parity for serial port. Defaults to none
  --timeout TIMEOUT     Response time-out seconds for MODBUS devices, Defaults
                        to 3.0
  -o, --export EXPORT   The file name to export references/registers
  --mqtt-version {3.1.1,5.0}
                        MQTT version. Defaults to MQTT v3.1.1
  --mqtt-host MQTT_HOST
                        MQTT server address. Skip MQTT setup if not specified
  --mqtt-port MQTT_PORT
                        1883 for non-TLS or 8883 for TLS, Defaults to 1883
  --mqtt-clientid MQTT_CLIENTID
                        MQTT client name, If qos > 0, set unique name for
                        multiple clients
  --mqtt-topic-prefix MQTT_TOPIC_PREFIX
                        (DEPRECATED) Topic prefix for MQTT
                        subscribing/publishing. Defaults to None
  --mqtt-publish-topic-pattern MQTT_PUBLISH_TOPIC_PATTERN
                        Topic pattern for MQTT publish. Use {{device_name}} as
                        placeholder for the device names in Modbus config.
                        Defaults to "modpoll/{{device_name}}/data"
  --mqtt-subscribe-topic-pattern MQTT_SUBSCRIBE_TOPIC_PATTERN
                        Topic pattern for MQTT subscribe. Defaults to
                        "modpoll/+/set"
  --mqtt-diagnostics-topic-pattern MQTT_DIAGNOSTICS_TOPIC_PATTERN
                        Topic pattern for MQTT diagnostics. Use
                        {{device_name}} as placeholder for the device names in
                        Modbus config. Defaults to
                        modpoll/{{device_name}}/diagnostics
  --mqtt-qos {0,1,2}    MQTT QoS value. Defaults to 0
  --mqtt-user MQTT_USER
                        Username for authentication (optional)
  --mqtt-pass MQTT_PASS
                        Password for authentication (optional)
  --mqtt-use-tls        Use TLS
  --mqtt-insecure       Use TLS without providing certificates
  --mqtt-cacerts MQTT_CACERTS
                        Path to ca keychain
  --mqtt-tls-version {tlsv1.2,tlsv1.1,tlsv1}
                        TLS protocol version, can be one of tlsv1.2 tlsv1.1 or
                        tlsv1
  --mqtt-single         Publish each value in a single topic. If not
                        specified, groups all values in one topic.
  --diagnostics-rate DIAGNOSTICS_RATE
                        Time in seconds as publishing period for each device
                        diagnostics
  --autoremove          Automatically remove poller if modbus communication
                        has failed 3 times.
  --loglevel {DEBUG,INFO,WARNING,ERROR,CRITICAL}
                        Set log level, Defaults to INFO
  --timestamp           Add timestamp to the result
  --delay DELAY         Time to delay sending first request in seconds after
                        connecting. Default to 0
  --framer {default,ascii,binary,rtu,socket}
                        The type of framer for modbus message. Use default
                        framer if not specified.
```