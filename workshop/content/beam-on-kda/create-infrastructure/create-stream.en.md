---
title: "Create a Kinesis data stream"
chapter: false
weight: 11
---

You start with creating a Kinesis data stream.

In Kinesis Data Stream a **shard** is the base throughput unit. One shard provides a capacity of 1MB/sec data input and 2MB/sec data output. One shard can support up to 1000 PUT records per second. You will specify the number of shards needed when you create the data stream.

1. Navigate to the [Kinesis Console](https://console.aws.amazon.com/kinesis)

1. If displayed, up press **Get Started** in the service welcome dialog

1. Select **Create data stream** to navigate to the Amazon Kinesis Data Stream service:
   ![](/images/kinesis-welcome-create-stream.png)

1. Choose `beam-workshop` as **Kinesis stream name**

1. Enter `4` as the **Number of shards**.

1. Select **Create Kinesis stream** at the bottom of the page
   ![](/images/kds-create-stream.png)

1. After a few moments, the data stream should have been created successfully and be in an _Active_ state
   ![](/images/kds-create-stream-active.png)