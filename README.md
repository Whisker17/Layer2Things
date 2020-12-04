# Layer2Things

This repo contains kinds of layer2 scheme in current market

## Catalogue

- [**Lightning Network**](https://github.com/Whisker17/Layer2Things/blob/main/lightningnetwork/README.md)

- [**Plasma**](https://github.com/Whisker17/Layer2Things/blob/main/plasma/README.md)
- [**State channel**](https://github.com/Whisker17/Layer2Things/blob/main/statechannel/README.md)
- [**Side chain**](https://github.com/Whisker17/Layer2Things/blob/main/sidechain/README.md)

- [**Rollup**](https://github.com/Whisker17/Layer2Things/blob/main/rollup/README.md)
- [**Reading Lists**](https://github.com/Whisker17/Layer2Things/blob/main/Reading_Lists.md)

- [**Difference between layer2 scheme**](#Difference-between-layer2-scheme)

### Difference between layer2 scheme

#### 对智能合约的支持

**首先，DeFi 应用需要支持智能合约，并且最好是灵活性较强的智能合约。**

![image](https://user-images.githubusercontent.com/12571049/98761196-e4ffa280-240f-11eb-91a0-308e0f62e858.png)

根据这一点， **状态通道** (State Channel) 和 **Plasma** 这两个方案，如非必要，**并不会**成为优先选择。因为他们对于智能合约的支持有限。

#### 资金安全性

DeFi 是重资产型的应用，意味着 Layer 2 方案要想胜任，就得有更好的确定性，更少的风险因素，DeFi 创建者也有余力可以在其他方面继续提升资金安全性。Layer 2 往往需要借助于验证人来充当中介角色，也因此带来了中间人风险。验证者是否有权限冻结资金甚至瓜分用户资金卷钱跑路？这一点，对于 DeFi 而言尤为重要。

![image](https://user-images.githubusercontent.com/12571049/98761294-17a99b00-2410-11eb-9763-ebc66ef7e387.png)

**SideChain**、Val**i**dum 这两类解决方案**对于中间验证人的依赖程度更高**，DeFi 在选择 Layer 2 方案时，需要慎重考虑。

#### 可用性

涉及到在资产处理效率的问题。

![image](https://user-images.githubusercontent.com/12571049/98761381-40ca2b80-2410-11eb-81c0-482beb29fc24.png)

**提现时间和交易是否可以即时确认**，是值得关注的两个方面。 Plasma 和 Optimistic rollups 的方案，从表中看到，提现时间预计较长。不过，如果引入了流动性提供者，相应提现时间会大大缩减，而 DeFi 方案目前通常都会有 LP 的设计，所以图中所示的 1 周提现时间尽管看来离奇得长，但是也只是理论预估而已，实现起来的实际时间会远小于此数值。

#### 性能

![image](https://user-images.githubusercontent.com/12571049/98761416-59d2dc80-2410-11eb-8c81-601875cbb032.png)