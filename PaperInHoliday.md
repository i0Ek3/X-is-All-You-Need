# Paper I Readed 


## 1. Federated Byzantine Agreement to Ensure Trustworthiness of Digital Manufacturing Platforms

**联邦拜占庭协议确保数字化制造平台的可靠性**<br>
> 在本文中，我们探讨了使用恒星共识协议（SCP）及其联邦拜占庭协议（FBA）算法来确保联合的，基于云的平台实例（节点）及其参与者之间的信任和声誉。 我们的方法基于联合共识机制，该机制承诺通过计算信任和数据复制来管理数据质量，而无需集中授权。 我们在NIMBLE云制造平台的基础上进行实验，该平台旨在通过由对等网络管理的联合平台服务支持B2B数字制造社区及其业务的增长。 我们讨论NIMBLE应用程序逻辑和Stellar共识逻辑之间的消息交换流程。

## 2. A Secure Sharding Protocol For Open Blockchains

**开放区块链的安全分片协议**<br>
> 加密货币，例如比特币和250个类似的替代币，其核心是区块链协议 - 一种分布式计算节点网络的机制，可以定期就一组新交易达成一致。设计安全的区块链协议依赖于安全性方面的开放性挑战，即设计可由拜占庭或任意恶意节点操纵的高度可扩展协议协议。比特币的区块链协议协议表现出安全性，但不能扩展：它目前每秒处理3-7次事务，无论手头的可用计算能力如何。
> 
> 在本文中，我们提出了一种新的分布式协议协议，用于无权限的区块链，称为ELASTICO。 ELASTICO与可用的挖掘计算几乎线性地缩放事务率：网络中的计算能力越大，每单位时间选择的事务块数越多。 ELASTICO的网络消息效率很高，并且能够容忍高达总计算能力四分之一的副攻击者。从技术上讲，ELASTICO将建立网络（安全地）统一划分或并行化为较小的委员会，每个委员会都处理一组不相交的交易（或“分片”）。虽然分片在非拜占庭设置中很常见，但ELASTICO是第一个安全分片协议的候选者，其存在拜占庭式的对话。我们在具有多达1,600个节点的Amazon EC2上的可扩展性实验证实了ELASTICO的理论扩展属性。

### core:我们的方法中的关键思想是将网络划分为较小的委员会，每个委员会处理一组不相交的交易（或“碎片”）。具体而言，委员会的数量在总的计算能力中接近线性增长。每个委员会都有相当少的成员，因此他们可以运行经典的拜占庭协议协议，以平行的方式决定他们商定的交易集。

## <del>3. Number of confirmation blocks for Bitcoin and GHOST consensus protocols on networks with delayed message delivery</del>
**<del>具有延迟消息传递的网络上比特币和GHOST共识协议的确认块数</del>**<br>
> <del>本文提出了三种方法，用于确定网络上比特币和GHOST所需数量的确认块，其中使用不同模型的延迟消息传递，考虑到更快的对抗性节点同步的可能性。对于GHOST，我们提出了第一个（据我们所知）严格的理论方法，它允许为给定的攻击者的哈希值和攻击成功概率获得所需数量的确认块。</del>

## 4. Mechanising Blockchain Consensus

**机制化区块链共识**<br>
> 我们提出了基于区块链的分布式共识协议的第一个形式化，并在交互式证明助手中对其一致性进行了机械化验证。我们的开发包括块森林数据结构的参考机械化，这是实现可证明正确的每节点协议逻辑所必需的。我们还定义了一个网络模型，以复制状态转换系统的形式实现协议。协议的执行是通过异步消息传递的小步操作语义建模的，其中包可以重新排列或重复。
> 
在这项工作中，我们关注全球系统安全的概念，证明了最终的一致性。为此，我们提供了一个关于块森林的纯函数实现的定理库，定义了一个归纳系统不变量，并表明在静态系统状态下，它对每个节点事务的状态形成了一个全局协议。分类帐。我们的发展是参数化的。实现了几个安全原语，例如哈希函数，证明对象的概念，验证器接受函数和分叉选择规则。我们精确地描述了这些假设的假设，以证明全球系统的共识，并讨论它们的充分性。本文中描述的所有结果都在Coq中正式化。

共识协议的目标是保证网络参与者同意。 事务发生的顺序。 这不是通过直接排序交易来实现的，而是通过将它们分组成块然后通过FCR-对块序列（链）的比较操作达成一致，从而产生区块链。

# 5. POSTER: Mining with Proof-of-Probability in Blockchain

**海报：在区块链中使用概率证明进行挖掘**<br>

> 随着对加密货币的兴趣增加，工作量证明（PoW）和利益证明（PoS）方法出现了问题，这是在区块链中获取加密货币的最具代表性的方法。 PoW方法是不经济的，PoS方法很容易被少数人垄断。 为了解决这个问题，本文介绍了一种概率证明（PoP）方法。 PoP是一种方法，其中每个节点对加密的实际散列以及一些假散列进行排序，然后第一个解密实际散列的节点创建块。 此外，在解密一个散列然后解密下一个散列以限制过度的计算能力竞争时使用等待时间。 此外，在所提出的PoP方法中，可以避免具有许多赌注的验证器的集中化。
> 
> **在所提出的PoP方法中，每个节点都有自己的散列排序算法。当尝试以块为单位创建事务信息时，加密的实际哈希值和一些假哈希值通过区块链网络分发。然后，每个节点通过自己的排序算法找到实际的哈希值。首先挖掘实际哈希的节点接收加密货币补偿。**

### Model Design

1）每个节点（A，B，C，D）都有自己的哈希排序算法。<br>
2）当事务发生时，它通过区块链网络发送加密的哈希和大量假哈希。<br>
3）每个节点使用自己的哈希排序算法优先化哈希值。<br>
4）节点将输入值放入有序散列中以找到满足计算的nonce值。 在假的情况下，您必须有等待时间来查找与下一个哈希对应的nonce值。<br>
5）找到与真实散列相对应的随机数的节点接收加密货币的补偿。<br>

### Algorithm 
1）当事务发生时，它发送加密的哈希和大量的假哈希。<br>
2）每个节点使用自己的哈希排序算法按挖掘优先级排序。<br>
3）创建块头并输入任何nonce值以执行SHA解密操作。<br>
4）如果不满足所需的模式，请调整nonce值以重复步骤3。<br>
5）如果满足所需的模式，则验证对应于散列的随机数是实际散列值的随机数。<br>
6）如果它不是真正的哈希值，请选择带有等待时间的下一个已排序哈希值，然后尝试步骤3。<br>
7）如果它被证明是一个真正的哈希值，它会为事务创建一个块。<br>

## 6. Conquering Generals: an NP-Hard Proof of Useful Work

**征服将军：有用工作的NP难题证明**<br>

> 最广泛采用的工作证明是Hashcash方案，最广泛部署的矿工是基于ASIC的。尽管Hashcash很受欢迎，但两个问题通常被确定为使用它。首先，该方案的高能耗被认为是浪费的，因为找到的解决方案没有提供有用的输出，其次，该方案的计算复杂性类别尚未正式知晓。基于这些不足，我们提出了一种新颖的工作证明系统，它实现了以下目标：
> 
- 为算法研究提供财政激励平台，旨在优化NP-Hard计算问题。这提供了间接洞察P Versus NP Clay Institute Mil-lennium问题，从而提供有用的输出。
- 在已知的硬计算复杂性类中构建挑战。
- 确保创建的工作证明包含ASIC硬件。
> 
我们的提议是一个混合的工作证明系统，最初使用Hashcash方案，并随后构建NP-Hard Travelmanman问题的实例。我们建立在其他人的立场上，以发展有用工作的证明。我们将我们的论文与相关工作区分开来，首先考虑当前对ASIC硬件的资本投入，从而将其纳入我们的提案中。

我们提出了一种混合的两轮有用工作证明方案，其具有确定的时间间隔，其在第一轮中继续使用ASIC硬件，并且随后构建NP-硬旅行推销员问题的实例。我们的混合方法确保了目前已经购买和部署的ASIC矿工的使用，从而避免了后一种浪费情况。

> “征服将军”这个名称是旅行商问题和拜占庭将军问题的结合，这些问题与工作证明中达成的共识有关。 我们将这项工作等同于一群将军在征服任务时所做的规划工作。 首先，他们进行侦察以确定他们想要推翻的城市（Hashcash阶段），然后他们建立征服城市的最佳秩序（TSP阶段）。


## 7. FruitChains: A Fair Blockchain

**FruitChains：一个公平的区块链**<br>

> 我们提出了一种新的区块链协议 - FruitChain协议，它满足与Nakamoto的协议（假设大部分是计算能力）相同的一致性和活跃性，并且另外是δ-近似公平：以极大的概率，控制计算能力的φ分数的任何诚实的一组玩家保证至少得到一小部分（1-δ）链的任何Ω（κ）长度δ段中的块（以及因此奖励）的φ（其中κ是安全参数）。因此，如果这个区块链协议被用作加密货币体系下的分类账，其中奖励和交易费用均匀分布在链条长度κ段的区块矿工之间，没有联盟控制少于大部分计算通过偏离协议，权力可以获得超过因子（1 +3δ）（即，诚实参与是0.5n联盟安全的3δ-Nash均衡）。最后，FruitChain协议可以减少采矿奖励的差异，从而显着减少（甚至消除）对采矿池的需求。

在这项工作中，我们引入了区块链协议公平性的概念：粗略地说，我们说区块链协议是公平的，如果使用φ部分计算资源的诚实参与者将获得至少φ分数的任何块 足够长的链条窗口。 （这种公平的概念可以被视为“理想链条质量”概念的强化形式，在[8,18]中考虑但未实现）更确切地说，我们说区块链协议是δ-近似公平的w.r.t. ρ攻击者，如果以极大的概率，任何诚实用户的φ分数联盟保证在链的每个足够长的窗口中至少获得块的（1-δ）φ分数，即使存在对手控制 到计算能力的ρ分数。 

我们的FruitChain协议将运行Nakamoto区块链协议的实例，但不是直接将记录存储在区块链内，而是将记录放在表示为f的“水果”中;这些水果本身需要解决一些工作证明，具有不同的硬度参数pf;另外，我们要求水果从链中的一个块“悬挂”，该块与记录水果的块不太“远” - 更具体地说，水果需要“指向”链中的较早块。距离含有它的块不太远（因此，水果不能“太久”开采） - 我们将这种水果称为最近的水果。在这个新的协议中，水果扮演“块”的角色 - 即，“橙色是新的块”1 - 因此链的质量根据果实来定义。

## 8. On the Security and Performance of Proof of Work Blockchains

**论工作区块链证明的安全性和性能**<br>

> 工作证明（PoW）驱动的区块链目前占现有数字加密货币总市值的90％以上。尽管比特币的安全规定已经得到了彻底的分析，但变体（分叉）PoW区块链（用不同的参数实例化）的安全保证在文献中并未引起太多关注。
在本文中，我们引入了一个新的定量框架来分析PoW区块链的各种共识和网络参数的安全性和性能影响。基于我们的框架，我们设计了双重支出和自私挖掘的最优对抗策略，同时考虑了现实世界的约束，如网络传播，不同的块大小，块生成间隔，信息传播机制以及日食攻击的影响。因此，我们的框架允许我们捕获现有的基于PoW的部署以及使用不同参数实例化的PoW区块链变体，并客观地比较其性能和安全性规定之间的权衡。

> 本文第三节介绍了针对比特币的两种攻击方法的MDP

## 9. RMBC: Randomized Mesh Blockchain Using DBFT Consensus Algorithm

**RMBC：使用DBFT共识算法的随机网格区块链**<br>
>  区块链是分散的网络系统，通过没有可信第三方的验证者的共识来验证交易的有效性。该机制确保透明地公开交易信息的交易完整性。因此，通过分散化，确保完整性和经济成本降低的特点，提高可靠性和效率，正在成为第四次工业革命的核心技术。但是，区块链的增长存在一些问题。应用于公共区块链的普遍使用的PoW（工作证明）一致性算法要求对价格进行补偿以便就交易的有效性达成一致。这样做的缺点是系统无法在没有补偿的情况下运行。此外，使用私有区块链的BFT（拜占庭容错）算法具有有限数量的可接受恶意用户。在这种情况下，如果用户串通恶意并超过有限数量，则拒绝该交易。在本文中，我们提出了一个智能管理系统和RMBC-DBFT（随机网格区块链多样性意见BFT）使安全交易能够解决上述问题。

为了解决这个问题，本文提出了利用**DBFT（意见多样性拜占庭容错）**算法应用RMBC（随机网格区块链）来解决上述问题的可能性。

PBFT算法是一种方法，即使恶意用户不遵守规定的规则，也能确保参与分布式系统的用户的协议正确。为了防止恶意用户做出错误的决定，交易是在3f + 1和5f + 1之类的预定义多数的协议下进行的。这意味着如果有三个恶意用户（f = 3），总用户数必须至少超过10才能获得正确的协议结果。

**这是一种结构，当大多数用户由小组组成时，大多数用户可能会串通并恶意改变该过程。因此，有第二个协议过程。第二个协议流程涉及对相关部门进行分组并将其分组。之后，RMBC从每个部门随机选择验证者，并进行第二次协议处理。此时，如果第一协议流程和第二协议流程彼此一致，则它将执行交易。如果它们不相同，则交易将被拒绝。如果我们比较两个过程，例如在同一组中的用户之间进行协议处理，并与在另一个组中随机选择的用户进行协议处理，后者似乎更客观，并且从其他组中随机选择的验证者可以判断交易从第三方的角度来看。因此，期望共谋的概率降低。**

当使用现有的区块链算法（例如PoW和BFT）时，可能会出现以下问题。首先，使用PoW，应该进行验证支付以平稳地操作系统。如果是BFT，恶意串通的可能性会增加，因为它是由一个小组组成的。因此，为了解决这些问题，本文提出了基于DBFT算法的RMBC，并提出了使用规定的公式不会发生恶意串通的可能性。此外，所提出的技术可以扩展像PoW这样的参与者的数量，并且可以期望比使用BFT算法的PoW更好的性能。

## 10. Inclusive Block Chain Protocols

**包含性块链协议**<br>

> 我们为链条提出了一种替代结构，允许以更高的速率进行操作。我们的结构由一个有向的非循环图块（块DAG）组成。 DAG结构是通过允许块引用多个前任来创建的，并允许更多“允许”的事务接受规则，即使来自看似冲突的块也包含事务。因此，系统可以容忍需要更长时间传播的更大块，并且可以增加事务量。
块链协议的另一个缺点是它们更喜欢更多连接的节点，这些节点可以更快地扩展块 - 更少的块冲突。我们表明，通过我们的系统，这种高度连接的矿工的优势大大减少。在消极方面，试图恶意逆转交易的攻击者可以尝试使用DAG结构的宽容性来降低攻击成本。我们提供了协议的安全性分析，并表明可以轻松应对此类尝试。

我们提出了包含性协议，该协议将离链块的内容集成到分类帐中。 我们的修改导致节点对行为改变的激励，导致吞吐量增加，并为弱矿工提供更好的回报。 我们未来工作的计划包括对交易授权政策和等待时间的额外分析以及自私采矿下的协议评估。

## 11. Proof of Stake versus Proof of Work

**股权证明与工作证明**

> 股权证明是数字货币的共识机制，可以替代比特币中使用的工作证明。 证明赌注方法的主要宣称的优点是缺乏昂贵的计算，因此，阻止了世代奖励的进入门槛较低。 在本报告中，我们研究了两种共识系统的优缺点，并表明现有的股权证明实施容易受到比特币和一般工作证明方法不太可能发生的攻击。

事务表示系统状态的原子更改。

Peercoin的共识机制结合了PoW和PoS，其中，工作证明用于分发新硬币，利益证明用于保护交易，即作为产生交易块的主要手段。

>为了提供区块链的稳定性，Peercoin定期使用广播检查点。 这种类型的广播引入了集中点。 虽然检查点存在于比特币协议[12]中，但它们可以被关闭并被硬编码到协议中而不是广播; 因此，比特币的检查点机制并不意味着集中化的风险。

Nxt是2013年开始的股权加密货币的纯粹证明。与Peercoin不同，Nxt不使用工作证明来创建新硬币;从创世块开始，系统中存在10亿个硬币（NXT）的全部可用供应量。因此，薄荷块的唯一动机是收取交易费用。

> Nxt中的事务与比特币事务完全不同，后者又导致其他协议差异[13]：Nxt事务没有锁定和解锁脚本。相反，Nxt协议使用帐户来编码交易的发件人和收件人。与比特币相比，这种限制严重限制了系统处理智能合约的能力。有各种类型的交易，例如信息，彩色硬币，数字商品等的特殊交易块中的事务数存在硬编码限制：不超过255.另一方面，块之间的平均时间为1分钟。所有事务都有一个到期时间（默认为24小时）。当到期时间过去时未包含在块中的事务将从内存池中删除，必须重新发送。

Novacoin是一种混合证明工作/证明利益加密货币的原则与Peer-coin完全相似。
> 主要区别是：Novacoin使用更保守的采矿奖励公式：奖励每64倍的难度减半[15]（与Peercoin的16倍相比）。稍微不同的方法基于同样的重量（替代币）用于防止（3）。 此外，赌注块证明的共同奖励取决于消耗的硬币年龄和PoS难度[16]。Novacoin中的硬币日重量与硬币年龄类似地计算，移位30天，上限为90个硬币日。

BlackCoin是一种混合加密货币，它使用工作证据进行财富的初始分配，现在仅依靠股权证明。 BlackCoin是唯一使用未经修改的股权证明方法的货币（2），根据该货币，用户的股权计算为他在硬币总供应中的份额[17]。 新的块平均每64秒铸造一次; 以每年1％的利息支付最低工资（这意味着BlackCoin是一种通货膨胀货币）。

BitShares是一种多态数字资产，可用于创建与特定市场挂钩的可替代资产（例如，美元）,BitShares的一个创新功能是其委托的利益一致性证明算法。 
> 代表性的BitShares股权证明依赖于证人的概念。利益相关者可以选择任意数量的证人来生成块。每个利益相关者的票数都等于他拥有的BitShares的数量;投票可以任意方式在证人之间分配。除了证人候选人之外，用户还选择他估计足以进行权力下放的一些证人。当然，用户不能投票给他认为必要的更多证人。
在对投票结果进行统计后，将选出前N名证人。 N被定义为满足至少50％的利益相关者投票的最小数量。选定的证人每两秒轮流生产一次。在每个N个证人轮到他之后，证人名单被洗牌，以便阻止犯罪者的命令不断变化。

混合PoW / PoS共识对于远程攻击是安全的，只要网络中有足够的散列功率即可。将PoW块包含在区块链中也可以防止第3节中描述的其他攻击。然而，由于股权证明通常被引入作为工作证明的替代方案，因此综合解决方案最终完全放弃PoW或削弱其角色。

Tendermint [30]是一个区块链的提议概念，由一个经过修改的股权共识证据保证。在Tendermint中，每个块都由验证器进行加密签名。验证者是通过将他的硬币锁定在绑定交易中而承诺履行职责的用户;每个验证人的投票权与锁定货币的数量成正比。在完成验证员职责后，用户通过发布未绑定的交易来解锁他的资金;然后以一定的延迟（非约束期）解锁资金。
如果该区块由持有至少2/3的所有投票权的验证方签署，则该区块被视为有效。因此，只有当一组具有1/3总投票权的验证者签署两个竞争链时才能发生分支。如果存在分支，则签署多个链的验证器可以由发布包含其恶意证据的证据事务的用户处罚，即，在两个链上的相同高度的块的数字签名。证据交易摧毁了行为不当的验证人的所有锁定资金。该逻辑可防止短程攻击（例如，第3.4节中描述的贿赂攻击）。但是，它并不能阻止远程攻击：具有2/3投票权的验证者可以在所有资金解锁后密谋发布区块链分支。为了避免远程攻击，可以引入禁止远程分叉的机制（如在Nxt中）。

Slasher是由以太坊建筑师之一Vitalik Buterin概述的混合PoS / PoW算法[31]。 与其他混合算法不同，Slasher专门使用工作证明来生成块; 每个块都使用PoW和PoS进行验证。

Casper是以太坊开发商Vlad Zamfir [32]提出的赌注算法的概念证明。 与Tendermint类似，Casper使用块验证器的概念。 验证器通过为每个块分配概率来对块进行下注; 相同高度的块的概率总和必须等于100％。 为了在每个高度选择一个块，验证器可能需要执行几个下注轮次，直到至少2/3的验证器以高概率（例如，99％）在某个块上下注。 为了抵抗多数人的攻击，卡斯帕通过扣留一代奖励和锁定资金来自行为不当的验证人来惩罚偏离协议的行为。

纯粹的股权证明方法带来了巨大的安全威胁，无法在工作系统（包括比特币）的证明中重新创建。这些问题是股权算法证明所固有的，因为股权共识的证据并非固定在物理世界中（参见工作证明中的哈希设备）。这就是为什么几乎所有依赖股权证明的货币都使用额外的机制来解决安全问题。

## 12. Bitcoin-NG: A Scalable Blockchain Protocol
**比特币NG：可扩展的区块链协议**<br>
> 比特币衍生的区块链协议具有固有的可扩展性限制，在吞吐量和延迟之间进行权衡，这阻碍了这种潜力的实现。本文介绍了Bitcoin-NG（下一代），一种旨在扩展的新区块链协议。 Bitcoin-NG是一种拜占庭容错区块链协议，对极端流失很有效，并且与比特币共享相同的信任模型。除了比特币NG之外，我们还介绍了几种新的衡量标准，用于量化类比特币区块链协议的安全性和效率。我们实施比特币NG并以比例运营比特币系统15％的大小进行大规模实验，使用两种协议的未更改客户端。这些实验证明，比特币NG可以最佳地扩展，带宽仅受单个节点容量的限制，而延迟仅受网络传播时间的限制。

但区块链协议面临着显着的可扩展性障碍。这些系统处理事务的最大速率受到两个参数选择的限制：块大小和块间隔。增加块大小可以提高吞吐量，但是由此产生的更大的块需要更长的时间才能在网络中传播。减少阻塞间隔可以减少延迟，但会导致系统不一致并且区块链需要重组的不稳定性。

我们提出了基于与比特币相同的信任模型的可扩展区块链协议Bitcoin-NG。比特币NG的延迟仅受网络传播延迟的限制，其带宽仅受各个节点处理能力的限制。 Bitcoin-NG通过将比特币的区块链操作分解为两个平面来实现这种性能提升：领导者选举和交易序列化。它将时间划分为时代，每个时代都有一个单一的领导者。与比特币一样，领导者选举是随机进行的，很少进行。一旦选择了领导者，它就有权单方面地对交易进行序列化，直到选择了新的领导者，标志着前者的时代结束。

> 总之，本文做出了三点贡献。首先，它概述了Bitcoin-NG可扩展区块链协议，与比特币保持比特币信任假设相比，它实现了更高的吞吐量和更低的延迟。其次，它引入了评估Nakamoto共识协议的定量指标。这些指标旨在以比特币衍生货币的参数选择为基础进行讨论。最后，它通过大规模实验量化比特币NG的稳健性和可扩展性。

比特币-NG并没有引入自私采矿策略的新漏洞，因此比特币NG对于采用不到1/4采矿能力的攻击者进行自私采矿具有弹性。因此，我们认为比特币NG的保证在中本共识的有效性方面与比特币的保证相似。

> 双倍支出双重支出攻击仍然是比特币NG的一个漏洞，尽管程度低于比特币。

# 13. Transactions as Proof-of-Stake
**交易作为股权证明**<br>
> 利益证明背后的概念是一个区块链应该由链中有经济利益的人保护。 本文将介绍一种新的利益证明方法，利用每笔交易的硬币销毁日来代替目前工作证明所提供的绝大多数安全性。 与之前只有一些节点有助于股权证明计算的现有Proof-of-Stake系统不同，我们提出了一种新的利益证明方法，其中所有生成交易的节点都有助于网络的安全性。 我们推测这样一个网络对已知的比特币或Peercoin攻击免疫。

分散式系统面临的挑战是找到一种方法，每隔几分钟将广播限制为最多一个或两个节点。我们将提出一种不依赖于采矿的解决方案。

硬币日表示自特定硬币在网络上最后一次交易以来的天数。在任何给定的时间点，存在有限数量的硬币日，并且它们在长期持有大量余额的人手中累积。因此，硬币日可以被视为网络中股份的代理。每次涉及这些硬币的交易都会销毁硬币日，因此无法重复使用。

在本文中，我们提供了一种简化的Proof-of-Stake算法，该算法允许网络的所有用户为网络安全做出贡献以抵御攻击。对于任何行为者而言，维持一个包含比公共交易分类账更多的硬币日的秘密区块链在经济上是不可行的。所提出的技术解决了51％的攻击，自私采矿攻击，并提供防止双重支出的保护，同时根本不需要采矿。

由于股权证明可以消除对采矿奖励的需求，因此它们也消除了对通货膨胀的需求，同时也消除了浪费的能源消耗以进行工作量证明。在一个拥有越来越多的块链的世界中，通过工作量证明的安全性变得支离破碎而没有合并挖掘，并且合并挖掘有其自身的开销。通过这种新的合并证明方法，不再需要合并挖掘，并且可以支持无限数量的块链，而不会影响任何单个链的潜在安全性。