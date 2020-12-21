## 评论系统


### 包含组件

- comment-service
  - 提供评论相关的接口，比如/get, /post, /delete
- comment-job
  - cache miss时，消费kafka回源指令消息，去mysql获取数据，并且build-cache
