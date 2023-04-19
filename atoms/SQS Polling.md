- When you consume messages from a queue using **short polling**, Amazon SQS samples a subset of its servers (based on a weighted random distribution) and returns messages from only those servers.
- When the wait time for the `ReceiveMessage` API action is greater than 0, **long polling** is in effect. It reduces the number of API calls and costs, but it does increase the latency.