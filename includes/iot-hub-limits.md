The following table lists the limits associated with the different service tiers (S1, S2, S3, F1). For information about the cost of each *unit* in each tier, see [IoT Hub Pricing](https://azure.microsoft.com/pricing/details/iot-hub/).

| Resource | S1 Standard | S2 Standard | S3 Standard | F1 Free |
| --- | --- | --- | --- | --- |
| Messages/day |400,000 |6,000,000 |300,000,000 |8,000 |
| Maximum units |200 |200 |10 |1 |

> [!NOTE]
> If you anticipate using more than 200 units with an S1 or S2 or 10 units with an S3 tier hub, contact Microsoft support.
> 
> 

The following table lists the limits that apply to IoT Hub resources:

| Resource | Limit |
| --- | --- |
| Maximum paid IoT hubs per Azure subscription |10 |
| Maximum free IoT hubs per Azure subscription |1 |
| Maximum number of device identities<br/> returned in a single call |1000 |
| IoT Hub message maximum retention for device-to-cloud messages |7 days |
| Maximum size of device-to-cloud message |256 KB |
| Maximum size of device-to-cloud batch |256 KB |
| Maximum messages in device-to-cloud batch |500 |
| Maximum size of cloud-to-device message |64 KB |
| Maximum TTL for cloud-to-device messages |2 days |
| Maximum delivery count for cloud-to-device <br/> messages |100 |
| Maximum delivery count for feedback messages <br/> in response to a cloud-to-device message |100 |
| Maximum TTL for feedback messages in <br/> response to a cloud-to-device message |2 days |
| Maximum size of device twin <br/> (tags, reported properties, and desired properties) | 8 KB |
| Maximum size of device twin string value | 512 bytes |
| Maximum depth of object in device twin | 5 |
| Maximum size of direct method payload | 8 KB |
| Job history maximum retention | 30 days |
| Maximum concurrent jobs | 10 (for S3), 5 for (S2), 1 (for S1) |
| Maximum additional endpoints | 10 (for S1, S2, S3) |
| Maximum message routing rules | 100 (for S1, S2, S3) |


> [!NOTE]
> If you need more than 10 paid IoT hubs in an Azure subscription, contact Microsoft support.
> 
> 

The IoT Hub service throttles requests when the following quotas are exceeded:

| Throttle | Per-hub value |
| --- | --- |
| Identity registry operations <br/> (create, retrieve, list, update, delete), <br/> individual or bulk import/export |5000/min/unit (for S3) <br/> 100/min/unit (for S1 and S2). |
| Device connections |6000/sec/unit (for S3), 120/sec/unit (for S2), 12/sec/unit (for S1). <br/>Minimum of 100/sec. |
| Device-to-cloud sends |6000/sec/unit (for S3), 120/sec/unit (for S2), 12/sec/unit (for S1). <br/>Minimum of 100/sec. |
| Cloud-to-device sends |5000/min/unit (for S3), 100/min/unit (for S1 and S2). |
| Cloud-to-device receives |50000/min/unit (for S3), 1000/min/unit (for S1 and S2). |
| File upload operations |5000 file upload notifications/min/unit (for S3), 100 file upload notifications/min/unit (for S1 and S2). <br/> 10000 SAS URIs can be out for an Azure Storage account at one time.<br/> 10 SAS URIs/device can be out at one time. |
| Direct methods | 1500/sec/unit (for S3), 30/sec/unit (for S2), 10/sec/unit (for S1) |
| Device twin reads | 50/sec/unit (for S3), Maximum of 10/sec or 1/sec/unit (for S2), 10/sec (for S1) |
| Device twin updates | 50/sec/unit (for S3), Maximum of 10/sec or 1/sec/unit (for S2), 10/sec (for S1) |
| Jobs operations <br/> (create, update, list, delete) | 5000/min/unit (for S3), 100/min/unit (for S2), 100/min/unit (for S1) |
| Jobs per-device operation throughput | 50/sec/unit (for S3), Maximum of 10/sec or 1/sec/unit (for S2), 10/sec (for S1) |