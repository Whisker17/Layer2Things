# RollupThings

This repo contains kinds of rollup scheme in current market

## Catalogue

- [**Rollup**](#Rollup)

- [**Optimistic Rollup**](#Optimistic-Rollup)
- [**ZK-Rollup**](#ZK-Rollup)
- [**Rollup 各方案对比**](#Rollup-各方案对比)

### Rollup

**Rollup 是一种可以对开放式合约（即，所有人都能看见并与之交互的合约）进行扩容的通用方法**。**在 Rollup 上，对合约的调用及其 argument（实际参数）都是作为调用数据（calldata）写在链上的，但是合约的实际计算和存储都是在链下完成的**。有人会在链上发布一个 assertion（断言），断言合约将要执行的一系列操作（例如要完成的支付）以及执行完成之后合约状态的哈希值。可以认为，这个发布上链的断言将所有的调用和结果都 “卷起来”（“rolling up”）成为单笔发送上链的交易。

不同的 Rollup 系统有所区别的地方在于**确保 assertion 正确性的方式**。包括：非交互型 rollup（如，ZK-Rollup）、一轮交互型 rollup（如， “optimistic rollup” 提案）和多轮交互型 rollup 等等。

### Optimistic Rollup

Optimistic Rollups（ORs）是二层网络构造的一种，它不在以太坊的基础层上运行，而是在其之上运行。 这使大规模运行智能合约成为可能，与此同时仍然受到以太坊的保护。 这些构造类似于 Plasma ，但是以等价于 Plasma 几乎无限的可扩展性来运行与 EVM 兼容的虚拟机，称为 OVM （乐观虚拟机），该虚拟机使 ORs 能够运行所有以太坊上可以进行的操作。

Optimistic Rollups 的名称源于解决方案的工作方式。 之所以使用“乐观”，是因为聚合器仅发布所需的最少信息而没有任何证据，前提是聚合器在没有欺诈的情况下运行，并且仅在发生欺诈时提供证据。 之所以使用 “Rollups” ，是因为交易以聚合的形式提交到主链（也就是说，它们是 roll-up 的）。

​																																					[**Read More**](https://github.com/Whisker17/Layer2Things/tree/main/rollup/oprollup/README.md)

### ZK-Rollup

虽然之前提出了 Plasma 的概念，但是由于 Plasma 本身存在的种种问题，为了提高二层网络的可扩展性，大家致力于研发更加用户友好和资源占用较少的解决方案。 ZK-Rollups 是为实现该目标而开发的解决方案之一。

​																																					[**Read More**](https://github.com/Whisker17/Layer2Things/blob/main/rollup/zkrollup/README.md)

### Rollup 各方案对比