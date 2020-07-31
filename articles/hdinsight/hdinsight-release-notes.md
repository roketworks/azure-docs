---
title: Release notes for Azure HDInsight 
description: Latest release notes for Azure HDInsight. Get development tips and details for Hadoop, Spark, R Server, Hive, and more.
author: hrasheed-msft
ms.author: hrasheed
ms.reviewer: jasonh
ms.custom: hdinsightactive
ms.service: hdinsight
ms.topic: conceptual
ms.date: 07/31/2020
---
# Azure HDInsight release notes

This article provides information about the **most recent** Azure HDInsight release updates. For information on earlier releases, see [HDInsight Release Notes Archive](hdinsight-release-notes-archive.md).

## Summary

Azure HDInsight is one of the most popular services among enterprise customers for open-source analytics on Azure.

## Release date: 07/30/2020

This release applies both for HDInsight 3.6 and 4.0. HDInsight release is made available to all regions over several days. The release date here indicates the first region release date. If you don't see below changes, wait for the release being live in your region in several days.

## New features
### Support for SparkCruise
SparkCruise is an automatic computation reuse system for Spark. It selects common subexpressions to materialize based on the past query workload. SparkCruise materializes these subexpressions as part of query processing and computation reuse is automatically applied in the background. You can benefit from SparkCruise without any modification to the Spark code.
 
### Support Hive View for HDInsight 4.0
Apache Ambari Hive View is designed to help you author, optimize, and execute Hive queries from your web browser. Hive View is supported natively for HDInsight 4.0 clusters starting from this release. It doesn't apply to existing clusters. You need drop and recreate the cluster to get the built-in Hive View.
 
### Support Tez View for HDInsight 4.0
Apache Tez View is used to track and debug the execution of Hive Tez job. Tez View is supported natively for HDInsight 4.0 starting from this release. It doesn't apply to existing clusters. You need to drop and recreate the cluster to get the built-in Tez View.

## Deprecation
### Deprecation of Spark 2.1 and 2.2 in HDInsight 3.6 Spark cluster
Starting from July 1 2020, customers cannot create new Spark clusters with Spark 2.1 and 2.2 on HDInsight 3.6. Existing clusters will run as is without the support from Microsoft. Consider to move to Spark 2.3 on HDInsight 3.6 by June 30 2020 to avoid potential system/support interruption.
 
### Deprecation of Spark 2.3 in HDInsight 4.0 Spark cluster
Starting from July 1 2020, customers cannot create new Spark clusters with Spark 2.3 on HDInsight 4.0. Existing clusters will run as is without the support from Microsoft. Consider moving to Spark 2.4 on HDInsight 4.0 by June 30 2020 to avoid potential system/support interruption.
 
### Deprecation of Kafka 1.1 in HDInsight 4.0 Kafka cluster
Starting from July 1 2020, customers will not be able to create new Kafka clusters with Kafka 1.1 on HDInsight 4.0. Existing clusters will run as is without the support from Microsoft. Consider moving to Kafka 2.1 on HDInsight 4.0 by June 30 2020 to avoid potential system/support interruption.

## Behavior changes
### Ambari stack version change
From this release, the Ambari version is changed from 2.x.x.x to 4.1. You can get the Ambari version from Ambari UI > About.

## Upcoming changes
No upcoming breaking changes that you need to pay attention to.

## Bug fixes
HDInsight continues to make cluster reliability and performance improvements. 

Below JIRAs are back ported for Hive:
* [HIVE-23619](https://issues.apache.org/jira/browse/HIVE-23619)
* [HIVE-21223](https://issues.apache.org/jira/browse/HIVE-21223)
* [HIVE-22599](https://issues.apache.org/jira/browse/HIVE-22599)
* [HIVE-22121](https://issues.apache.org/jira/browse/HIVE-22121)
* [HIVE-22136](https://issues.apache.org/jira/browse/HIVE-22136)
* [HIVE-18786](https://issues.apache.org/jira/browse/HIVE-18786)

## Component version change
No component version change for this release. You can find the current component versions for HDInsight 4.0 and HDInsight 3.6 in [this doc](https://docs.microsoft.com/azure/hdinsight/hdinsight-component-versioning#apache-hadoop-components-available-with-different-hdinsight-versions).