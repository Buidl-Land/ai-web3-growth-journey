+--------------------------------------------------+
|                  用户界面 (前端)                   |
|  +------------------------------------------+    |
|  |         React.js / Next.js App          |    |
|  +------------------------------------------+    |
|       |                  ↑                      |
|       | 提交问题+支付        | 接收回答              |
|       ↓                  |                      |
+--------------------------------------------------+
            |                  ↑
            | Web3 / ethers.js | 
            ↓                  |
+--------------------------------------------------+
|                区块链网络 (智能合约)                 |
|  +------------------------------------------+    |
|  |              ConsultToken               |    |
|  |      (ERC-20 代币用于支付AI服务)            |    |
|  +------------------------------------------+    |
|                        |                        |
|  +------------------------------------------+    |
|  |              AIConsultant               |    |
|  |   (处理请求、支付和存储AI回答的智能合约)        |    |
|  +------------------------------------------+    |
|       |                  ↑                      |
|       | 请求事件          | 回答提交               |
|       ↓                  |                      |
+--------------------------------------------------+
            |                  ↑
            | Oracle / MCP    |
            ↓                  |
+--------------------------------------------------+
|                  后端 MCP 服务                    |
|  +------------------------------------------+    |
|  |        Node.js / Express Server         |    |
|  +------------------------------------------+    |
|       |                  ↑                      |
|       | 请求AI回答        | 接收AI回答              |
|       ↓                  |                      |
+--------------------------------------------------+
            |                  ↑
            | API 调用         |
            ↓                  |
+--------------------------------------------------+
|                  AI 服务提供商                    |
|  +------------------------------------------+    |
|  |      Claude / GPT / 自定义AI模型           |    |
|  +------------------------------------------+    |
+--------------------------------------------------+
``` 