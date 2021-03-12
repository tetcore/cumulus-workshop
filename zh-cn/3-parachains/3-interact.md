# 与您的平行链交互

启动和注册平行链的全部意义在于我们可以提交交易给平行链以及与它们交互。


## 连接 Apps UI

我们已经将Apps UI连接到中继链节点。现在我们也可以连接到平行链的收集者节点。在新的浏览器窗口中打开另一个Apps示例，并将其连接到相应的端点。
如果您已经按照这些说明进行了操作，您可以在https://polkadot.js.org/apps/#/?rpc=ws://localhost:9977连接到Alice的节点。


## 添加自定义类型

收集者已经引入了前端不知道的自定义数据类型。为了正确的解码交易信息，我们必须告诉前端这些类型。在`Settings` -> `Developer` 栏中输入下面的json。


```json
{
  "Address": "AccountId",
  "LookupSource": "AccountId"
}
```

## 提交交易

您可以进行一些简单的代币转账以确保平行链正常运行。您也可以通过提交`Extrinsics` -> `System` -> `remark`来进行链上的备注。


如果交易事务像期待中的运行的话，您就有了一个正在工作的平行链！在下一节中我们将学习关于跨链转账。
