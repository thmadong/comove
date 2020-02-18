# Co-Move
Co-Move is a short name for Cosmos-Move, A Smart Contract Framework on Cosmos Blockchain.

In order to make sure what I write is what I am really want to write, I have to write this document in Chinese. For English readers, my friend Google Translate will help you and he can do a better job in translation than I do.

## 背景

[Cosmos](https://cosmos.network) 是知名的跨链区块链项目。它不仅提供了区块链跨链的解决方案，而且还提供了一个非常优秀的区块链开发框架 - [Cosmos-SDK](https://github.com/cosmos/cosmos-sdk)。在Cosmos的设计理念里，你可以为每一个应用开发一个完全自主可控的区块链。但是在很多DApp的使用场景，许多开发者并不想开发一个条独立的区块链，运营它，因为这个需要很多资源才能做好，他们只想在某一个成熟区块链（例如：Cosmos-Hub）上去做一些功能扩展，所以，智能合约在很多场景下还是有必要的。

[Move](https://github.com/libra/libra/tree/master/language) 是由Facebook Libra创造的专用智能合约编程语言，它小巧，安全，强大。但是他现在还不成熟，还在紧张的开发中，不过，我深信它会是最好的智能合约语言。

[CosmWasm](https://github.com/cosmwasm/) 它是首个Cosmos上的智能合约解决方案，感谢Ethan Frey以及其他贡献者在这一领域的探索和贡献。

## 关于 GO 和 Rust

Cosmos 使用Go语言开发，而Move VM使用的Rust语言开发。所以，要实现Co-Move, 我们需要解决的第一个问题就是跨语言调用的问题。现在主要有两个可行的方案可供选择：

* CGO + Rust FFI 如果你感兴趣，你可以在[这里](https://github.com/medimatrix/rust-plus-golang)了解更多信息。
* Web Assembly

我个人倾向于采用CGO+FFI的方案，据我了解其实Web Assembly的虚拟机也是使用CGO来做的，所以，我希望这个方案更直接一个点。不管怎么说，Move VM in WebAssembly VM看起来要复杂一点，虽然这么说可能不太科学。

## 设计思路


## 赞助商

* ping.pub

## Contributors

* liangping

