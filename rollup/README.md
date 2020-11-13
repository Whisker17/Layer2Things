# RollupThings

This repo contains kinds of rollup scheme in current market

> Rollup 是一种可以对开放式合约（即所有人都能看见并与之交互的合约）进行扩容的通用方法。在 Rollup 上，对合约的调用及其 argument（实际参数）都是作为**调用数据（calldata）**写在链上的，但是合约的**实际计算和存储都是在链下完成的**。有人会在链上发布一个 **assertion（断言）**，断言合约将要执行的一系列操作（例如要完成的支付）以及执行完成之后合约状态的哈希值。可以认为，这个发布上链的断言将所有的调用和结果都  “卷起来”（“rolling up”）成为单笔发送上链的交易。
>
不同的 Rollup 系统有所区别的地方在于**确保 assertion 正确性的方式**。这里有三种基本方法：
* **非交互型 rollup**（如，ZK-Rollup）
* **一轮交互型 rollup**（如， “optimistic rollup” 提案）
* **多轮交互型 rollup** 



## Optimistic Rollup



## ZK-Rollup