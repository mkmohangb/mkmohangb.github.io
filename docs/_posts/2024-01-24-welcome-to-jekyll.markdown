---
layout: post
title:  "Report "
date:   2024-01-24 13:10:49 +0530
categories: daily log
---
Apache Kafka - Rust

[rust-rdkafka][rust-rdkafka] is a Rust client library for Apache Kafka. It is based off librdkafka(a c/c++ library).

Tried the simple producer/consumer clients provided as part of the examples. For the broker, there is a docker-compose file which launches one using Zookeeper based on images hosted by Confluent inc.
Had an issue with creating consumer because of reading a config value "max.poll.interval.ms" which had a spurious null character like so "30000\0" hence the parsing of string to a number was failing. Tried using the nvim-dap based debugger to figure out the problem. But somehow had issues printing variable values and finally fell back to using the plain old println! macro.


[rust-rdkafka]: https://github.com/fede1024/rust-rdkafka/
