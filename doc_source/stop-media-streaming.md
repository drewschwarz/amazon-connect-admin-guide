# Contact Block: Stop Media Streaming<a name="stop-media-streaming"></a>

## In contact flow types<a name="stop-media-streaming-types"></a>

You can use this block in the following [contact flow types](create-contact-flow.md#contact-flow-types):
+ Generic Contact flow
+ Customer Queue flow
+ Customer Whisper flow
+ Outbound Whisper flow
+ Agent Whisper flow
+ Transfer to Agent flow
+ Transfer to Queue flow

## Description<a name="stop-media-streaming-description"></a>
+ Stops capturing customer audio after it is started with a **Start media streaming** block\.
+ You must use a **Stop media streaming** block to stop media streaming\.

## Properties<a name="stop-media-streaming-properties"></a>

This block doesn't have any properties\.

## Configuration tips<a name="stop-media-streaming-tips"></a>
+ You must enable live media streaming in your instance to successfully capture customer audio\. For instructions, see [Capture Customer Audio: Live Media Streaming](customer-voice-streams.md)\.
+ Customer audio is captured until a **Stop media streaming** block is invoked, even if the contact is passed to another contact flow\.
+ If this block is triggered during a chat conversation, the contact is routed down the **Error** branch\.

## Configured block<a name="stop-media-streaming-configured"></a>

When this block is configured, it looks similar to the following image:

![\[Image NOT FOUND\]](http://docs.aws.amazon.com/connect/latest/adminguide/images/stop-media-streaming-configured.png)

## Sample flows<a name="stop-media-streaming-samples"></a>

[Example Contact Flow for Testing Live Media Streaming](use-media-streams-blocks.md) 