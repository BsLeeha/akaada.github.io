整了一些场景使用误区。
# Message rates 不断变化，Queued messages 始终显示为 0
<img width="928" alt="image" src="https://github.com/zhi-qiu-yi/zhi-qiu-yi.github.io/assets/32633065/8b55217b-b5b8-4981-ba2d-420bd2cfcfbe">
Queued messages 显示的是**队列堆积的消息**，只有消费速率跟不上生产速率时，才会有堆积消息。
右边的三个 tab 是堆积消息的三种状态：

- Ready: 在队列中，可以被消费者消费
- Unacked: 消费者消费了该消息，但是没有返回 ack 响应
- Total: 前两者之合