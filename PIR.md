# ★ Paper I Readed ★

There are some English papers I readed which talk about blockchain consensus algorithm.


### 1. Federated Byzantine Agreement to Ensure Trustworthiness of Digital Manufacturing Platforms

**联邦拜占庭协议确保数字化制造平台的可靠性**

> 在本文中，我们探讨了使用恒星共识协议（SCP）及其联邦拜占庭协议（FBA）算法来确保联合的，基于云的平台实例（节点）及其参与者之间的信任和声誉。 我们的方法基于联合共识机制，该机制承诺通过计算信任和数据复制来管理数据质量，而无需集中授权。 我们在NIMBLE云制造平台的基础上进行实验，该平台旨在通过由对等网络管理的联合平台服务支持B2B数字制造社区及其业务的增长。 我们讨论NIMBLE应用程序逻辑和Stellar共识逻辑之间的消息交换流程。


### 2. A Secure Sharding Protocol For Open Blockchains

**开放区块链的安全分片协议**

> 加密货币，例如比特币和250个类似的替代币，其核心是区块链协议 - 一种分布式计算节点网络的机制，可以定期就一组新交易达成一致。设计安全的区块链协议依赖于安全性方面的开放性挑战，即设计可由拜占庭或任意恶意节点操纵的高度可扩展协议协议。比特币的区块链协议协议表现出安全性，但不能扩展：它目前每秒处理3-7次事务，无论手头的可用计算能力如何。

> 在本文中，我们提出了一种新的分布式协议协议，用于无权限的区块链，称为ELASTICO。 ELASTICO与可用的挖掘计算几乎线性地缩放事务率：网络中的计算能力越大，每单位时间选择的事务块数越多。 ELASTICO的网络消息效率很高，并且能够容忍高达总计算能力四分之一的副攻击者。从技术上讲，ELASTICO将建立网络（安全地）统一划分或并行化为较小的委员会，每个委员会都处理一组不相交的交易（或“分片”）。虽然分片在非拜占庭设置中很常见，但ELASTICO是第一个安全分片协议的候选者，其存在拜占庭式的对话。我们在具有多达1,600个节点的Amazon EC2上的可扩展性实验证实了ELASTICO的理论扩展属性。

我们的方法中的关键思想是将网络划分为较小的委员会，每个委员会处理一组不相交的交易（或“碎片”）。具体而言，委员会的数量在总的计算能力中接近线性增长。每个委员会都有相当少的成员，因此他们可以运行经典的拜占庭协议协议，以平行的方式决定他们商定的交易集。


### <del>3. Number of confirmation blocks for Bitcoin and GHOST consensus protocols on networks with delayed message delivery</del>

**<del>具有延迟消息传递的网络上比特币和GHOST共识协议的确认块数</del>**

> <del>本文提出了三种方法，用于确定网络上比特币和GHOST所需数量的确认块，其中使用不同模型的延迟消息传递，考虑到更快的对抗性节点同步的可能性。对于GHOST，我们提出了第一个（据我们所知）严格的理论方法，它允许为给定的攻击者的哈希值和攻击成功概率获得所需数量的确认块。</del>


### 4. Mechanising Blockchain Consensus

**机制化区块链共识**

> 我们提出了基于区块链的分布式共识协议的第一个形式化，并在交互式证明助手中对其一致性进行了机械化验证。我们的开发包括块森林数据结构的参考机械化，这是实现可证明正确的每节点协议逻辑所必需的。我们还定义了一个网络模型，以复制状态转换系统的形式实现协议。协议的执行是通过异步消息传递的小步操作语义建模的，其中包可以重新排列或重复。

在这项工作中，我们关注全球系统安全的概念，证明了最终的一致性。为此，我们提供了一个关于块森林的纯函数实现的定理库，定义了一个归纳系统不变量，并表明在静态系统状态下，它对每个节点事务的状态形成了一个全局协议。分类帐。我们的发展是参数化的。实现了几个安全原语，例如哈希函数，证明对象的概念，验证器接受函数和分叉选择规则。我们精确地描述了这些假设的假设，以证明全球系统的共识，并讨论它们的充分性。本文中描述的所有结果都在Coq中正式化。

共识协议的目标是保证网络参与者同意。 事务发生的顺序。 这不是通过直接排序交易来实现的，而是通过将它们分组成块然后通过FCR-对块序列（链）的比较操作达成一致，从而产生区块链。


### [★] 5. POSTER: Mining with Proof-of-Probability in Blockchain

**海报：在区块链中使用概率证明进行挖掘**

> 随着对加密货币的兴趣增加，工作量证明（PoW）和利益证明（PoS）方法出现了问题，这是在区块链中获取加密货币的最具代表性的方法。 PoW方法是不经济的，PoS方法很容易被少数人垄断。 为了解决这个问题，本文介绍了一种概率证明（PoP）方法。 PoP是一种方法，其中每个节点对加密的实际散列以及一些假散列进行排序，然后第一个解密实际散列的节点创建块。 此外，在解密一个散列然后解密下一个散列以限制过度的计算能力竞争时使用等待时间。 此外，在所提出的PoP方法中，可以避免具有许多赌注的验证器的集中化。

> **在所提出的PoP方法中，每个节点都有自己的散列排序算法。当尝试以块为单位创建事务信息时，加密的实际哈希值和一些假哈希值通过区块链网络分发。然后，每个节点通过自己的排序算法找到实际的哈希值。首先挖掘实际哈希的节点接收加密货币补偿。**


#### Model Design

1）每个节点（A，B，C，D）都有自己的哈希排序算法。<br>
2）当事务发生时，它通过区块链网络发送加密的哈希和大量假哈希。<br>
3）每个节点使用自己的哈希排序算法优先化哈希值。<br>
4）节点将输入值放入有序散列中以找到满足计算的nonce值。 在假的情况下，您必须有等待时间来查找与下一个哈希对应的nonce值。<br>
5）找到与真实散列相对应的随机数的节点接收加密货币的补偿。<br>

#### Algorithm 
1）当事务发生时，它发送加密的哈希和大量的假哈希。<br>
2）每个节点使用自己的哈希排序算法按挖掘优先级排序。<br>
3）创建块头并输入任何nonce值以执行SHA解密操作。<br>
4）如果不满足所需的模式，请调整nonce值以重复步骤3。<br>
5）如果满足所需的模式，则验证对应于散列的随机数是实际散列值的随机数。<br>
6）如果它不是真正的哈希值，请选择带有等待时间的下一个已排序哈希值，然后尝试步骤3。<br>
7）如果它被证明是一个真正的哈希值，它会为事务创建一个块。<br>


### 6. Conquering Generals: an NP-Hard Proof of Useful Work

**征服将军：有用工作的NP难题证明**

> 最广泛采用的工作证明是Hashcash方案，最广泛部署的矿工是基于ASIC的。尽管Hashcash很受欢迎，但两个问题通常被确定为使用它。首先，该方案的高能耗被认为是浪费的，因为找到的解决方案没有提供有用的输出，其次，该方案的计算复杂性类别尚未正式知晓。基于这些不足，我们提出了一种新颖的工作证明系统，它实现了以下目标：
> 
- 为算法研究提供财政激励平台，旨在优化NP-Hard计算问题。这提供了间接洞察P Versus NP Clay Institute Mil-lennium问题，从而提供有用的输出。
- 在已知的硬计算复杂性类中构建挑战。
- 确保创建的工作证明包含ASIC硬件。
> 
我们的提议是一个混合的工作证明系统，最初使用Hashcash方案，并随后构建NP-Hard Travelmanman问题的实例。我们建立在其他人的立场上，以发展有用工作的证明。我们将我们的论文与相关工作区分开来，首先考虑当前对ASIC硬件的资本投入，从而将其纳入我们的提案中。

我们提出了一种混合的两轮有用工作证明方案，其具有确定的时间间隔，其在第一轮中继续使用ASIC硬件，并且随后构建NP-硬旅行推销员问题的实例。我们的混合方法确保了目前已经购买和部署的ASIC矿工的使用，从而避免了后一种浪费情况。

> “征服将军”这个名称是旅行商问题和拜占庭将军问题的结合，这些问题与工作证明中达成的共识有关。 我们将这项工作等同于一群将军在征服任务时所做的规划工作。 首先，他们进行侦察以确定他们想要推翻的城市（Hashcash阶段），然后他们建立征服城市的最佳秩序（TSP阶段）。


### 7. FruitChains: A Fair Blockchain

**FruitChains：一个公平的区块链**

> 我们提出了一种新的区块链协议 - FruitChain协议，它满足与Nakamoto的协议（假设大部分是计算能力）相同的一致性和活跃性，并且另外是δ-近似公平：以极大的概率，控制计算能力的φ分数的任何诚实的一组玩家保证至少得到一小部分（1-δ）链的任何Ω（κ）长度δ段中的块（以及因此奖励）的φ（其中κ是安全参数）。因此，如果这个区块链协议被用作加密货币体系下的分类账，其中奖励和交易费用均匀分布在链条长度κ段的区块矿工之间，没有联盟控制少于大部分计算通过偏离协议，权力可以获得超过因子（1 +3δ）（即，诚实参与是0.5n联盟安全的3δ-Nash均衡）。最后，FruitChain协议可以减少采矿奖励的差异，从而显着减少（甚至消除）对采矿池的需求。

在这项工作中，我们引入了区块链协议公平性的概念：粗略地说，我们说区块链协议是公平的，如果使用φ部分计算资源的诚实参与者将获得至少φ分数的任何块 足够长的链条窗口。（这种公平的概念可以被视为“理想链条质量”概念的强化形式）更确切地说，我们说区块链协议是δ-近似公平的w.r.t. ρ攻击者，如果以极大的概率，任何诚实用户的φ分数联盟保证在链的每个足够长的窗口中至少获得块的（1-δ）φ分数，即使存在对手控制 到计算能力的ρ分数。 

我们的FruitChain协议将运行Nakamoto区块链协议的实例，但不是直接将记录存储在区块链内，而是将记录放在表示为f的“水果”中;这些水果本身需要解决一些工作证明，具有不同的硬度参数pf;另外，我们要求水果从链中的一个块“悬挂”，该块与记录水果的块不太“远” - 更具体地说，水果需要“指向”链中的较早块。距离含有它的块不太远（因此，水果不能“太久”开采） - 我们将这种水果称为最近的水果。在这个新的协议中，水果扮演“块”的角色 - 即，“橙色是新的块”1 - 因此链的质量根据果实来定义。


### 8. On the Security and Performance of Proof of Work Blockchains

**论工作区块链证明的安全性和性能**

> 工作证明（PoW）驱动的区块链目前占现有数字加密货币总市值的90％以上。尽管比特币的安全规定已经得到了彻底的分析，但变体（分叉）PoW区块链（用不同的参数实例化）的安全保证在文献中并未引起太多关注。
> 
在本文中，我们引入了一个新的定量框架来分析PoW区块链的各种共识和网络参数的安全性和性能影响。基于我们的框架，我们设计了双重支出和自私挖掘的最优对抗策略，同时考虑了现实世界的约束，如网络传播，不同的块大小，块生成间隔，信息传播机制以及日食攻击的影响。因此，我们的框架允许我们捕获现有的基于PoW的部署以及使用不同参数实例化的PoW区块链变体，并客观地比较其性能和安全性规定之间的权衡。

> 本文第三节介绍了针对比特币的两种攻击方法的MDP


### 9. RMBC: Randomized Mesh Blockchain Using DBFT Consensus Algorithm

**RMBC：使用DBFT共识算法的随机网格区块链**

>  区块链是分散的网络系统，通过没有可信第三方的验证者的共识来验证交易的有效性。该机制确保透明地公开交易信息的交易完整性。因此，通过分散化，确保完整性和经济成本降低的特点，提高可靠性和效率，正在成为第四次工业革命的核心技术。但是，区块链的增长存在一些问题。应用于公共区块链的普遍使用的PoW（工作证明）一致性算法要求对价格进行补偿以便就交易的有效性达成一致。这样做的缺点是系统无法在没有补偿的情况下运行。此外，使用私有区块链的BFT（拜占庭容错）算法具有有限数量的可接受恶意用户。在这种情况下，如果用户串通恶意并超过有限数量，则拒绝该交易。在本文中，我们提出了一个智能管理系统和RMBC-DBFT（随机网格区块链多样性意见BFT）使安全交易能够解决上述问题。

为了解决这个问题，本文提出了利用**DBFT（意见多样性拜占庭容错）**算法应用RMBC（随机网格区块链）来解决上述问题的可能性。

PBFT算法是一种方法，即使恶意用户不遵守规定的规则，也能确保参与分布式系统的用户的协议正确。为了防止恶意用户做出错误的决定，交易是在3f + 1和5f + 1之类的预定义多数的协议下进行的。这意味着如果有三个恶意用户（f = 3），总用户数必须至少超过10才能获得正确的协议结果。

**这是一种结构，当大多数用户由小组组成时，大多数用户可能会串通并恶意改变该过程。因此，有第二个协议过程。第二个协议流程涉及对相关部门进行分组并将其分组。之后，RMBC从每个部门随机选择验证者，并进行第二次协议处理。此时，如果第一协议流程和第二协议流程彼此一致，则它将执行交易。如果它们不相同，则交易将被拒绝。如果我们比较两个过程，例如在同一组中的用户之间进行协议处理，并与在另一个组中随机选择的用户进行协议处理，后者似乎更客观，并且从其他组中随机选择的验证者可以判断交易从第三方的角度来看。因此，期望共谋的概率降低。**

当使用现有的区块链算法（例如PoW和BFT）时，可能会出现以下问题。首先，使用PoW，应该进行验证支付以平稳地操作系统。如果是BFT，恶意串通的可能性会增加，因为它是由一个小组组成的。因此，为了解决这些问题，本文提出了基于DBFT算法的RMBC，并提出了使用规定的公式不会发生恶意串通的可能性。此外，所提出的技术可以扩展像PoW这样的参与者的数量，并且可以期望比使用BFT算法的PoW更好的性能。


### 10. Inclusive Block Chain Protocols

**包含性块链协议**

> 我们为链条提出了一种替代结构，允许以更高的速率进行操作。我们的结构由一个有向的非循环图块（块DAG）组成。 DAG结构是通过允许块引用多个前任来创建的，并允许更多“允许”的事务接受规则，即使来自看似冲突的块也包含事务。因此，系统可以容忍需要更长时间传播的更大块，并且可以增加事务量。
> 
块链协议的另一个缺点是它们更喜欢更多连接的节点，这些节点可以更快地扩展块更少的块冲突。我们表明，通过我们的系统，这种高度连接的矿工的优势大大减少。在消极方面，试图恶意逆转交易的攻击者可以尝试使用DAG结构的宽容性来降低攻击成本。我们提供了协议的安全性分析，并表明可以轻松应对此类尝试。

我们提出了包含性协议，该协议将离链块的内容集成到分类帐中。 我们的修改导致节点对行为改变的激励，导致吞吐量增加，并为弱矿工提供更好的回报。 我们未来工作的计划包括对交易授权政策和等待时间的额外分析以及自私采矿下的协议评估。


### 11. Proof of Stake versus Proof of Work

**股权证明与工作证明**

> 股权证明是数字货币的共识机制，可以替代比特币中使用的工作证明。 证明赌注方法的主要宣称的优点是缺乏昂贵的计算，因此，阻止了世代奖励的进入门槛较低。 在本报告中，我们研究了两种共识系统的优缺点，并表明现有的股权证明实施容易受到比特币和一般工作证明方法不太可能发生的攻击。

事务表示系统状态的原子更改。

Peercoin的共识机制结合了PoW和PoS，其中，工作证明用于分发新硬币，利益证明用于保护交易，即作为产生交易块的主要手段。

> 为了提供区块链的稳定性，Peercoin定期使用广播检查点。 这种类型的广播引入了集中点。 虽然检查点存在于比特币协议中，但它们可以被关闭并被硬编码到协议中而不是广播; 因此，比特币的检查点机制并不意味着集中化的风险。

Nxt是2013年开始的股权加密货币的纯粹证明。与Peercoin不同，Nxt不使用工作证明来创建新硬币;从创世块开始，系统中存在10亿个硬币（NXT）的全部可用供应量。因此，薄荷块的唯一动机是收取交易费用。

> Nxt中的事务与比特币事务完全不同，后者又导致其他协议差异：Nxt事务没有锁定和解锁脚本。相反，Nxt协议使用帐户来编码交易的发件人和收件人。与比特币相比，这种限制严重限制了系统处理智能合约的能力。有各种类型的交易，例如信息，彩色硬币，数字商品等的特殊交易块中的事务数存在硬编码限制：不超过255.另一方面，块之间的平均时间为1分钟。所有事务都有一个到期时间（默认为24小时）。当到期时间过去时未包含在块中的事务将从内存池中删除，必须重新发送。

Novacoin是一种混合证明工作/证明利益加密货币的原则与Peer-coin完全相似。

> 主要区别是：Novacoin使用更保守的采矿奖励公式：奖励每64倍的难度减半（与Peercoin的16倍相比）。稍微不同的方法基于同样的重量（替代币）用于防止（3）。 此外，赌注块证明的共同奖励取决于消耗的硬币年龄和PoS难度。Novacoin中的硬币日重量与硬币年龄类似地计算，移位30天，上限为90个硬币日。

BlackCoin是一种混合加密货币，它使用工作证据进行财富的初始分配，现在仅依靠股权证明。 BlackCoin是唯一使用未经修改的股权证明方法的货币（2），根据该货币，用户的股权计算为他在硬币总供应中的份额。 新的块平均每64秒铸造一次; 以每年1％的利息支付最低工资（这意味着BlackCoin是一种通货膨胀货币）。

BitShares是一种多态数字资产，可用于创建与特定市场挂钩的可替代资产（例如，美元）,BitShares的一个创新功能是其委托的利益一致性证明算法。 

> 代表性的BitShares股权证明依赖于证人的概念。利益相关者可以选择任意数量的证人来生成块。每个利益相关者的票数都等于他拥有的BitShares的数量;投票可以任意方式在证人之间分配。除了证人候选人之外，用户还选择他估计足以进行权力下放的一些证人。当然，用户不能投票给他认为必要的更多证人。
在对投票结果进行统计后，将选出前N名证人。 N被定义为满足至少50％的利益相关者投票的最小数量。选定的证人每两秒轮流生产一次。在每个N个证人轮到他之后，证人名单被洗牌，以便阻止犯罪者的命令不断变化。

混合PoW / PoS共识对于远程攻击是安全的，只要网络中有足够的散列功率即可。将PoW块包含在区块链中也可以防止第3节中描述的其他攻击。然而，由于股权证明通常被引入作为工作证明的替代方案，因此综合解决方案最终完全放弃PoW或削弱其角色。

Tendermint是一个区块链的提议概念，由一个经过修改的股权共识证据保证。在Tendermint中，每个块都由验证器进行加密签名。验证者是通过将他的硬币锁定在绑定交易中而承诺履行职责的用户;每个验证人的投票权与锁定货币的数量成正比。在完成验证员职责后，用户通过发布未绑定的交易来解锁他的资金;然后以一定的延迟（非约束期）解锁资金。

如果该区块由持有至少2/3的所有投票权的验证方签署，则该区块被视为有效。因此，只有当一组具有1/3总投票权的验证者签署两个竞争链时才能发生分支。如果存在分支，则签署多个链的验证器可以由发布包含其恶意证据的证据事务的用户处罚，即，在两个链上的相同高度的块的数字签名。证据交易摧毁了行为不当的验证人的所有锁定资金。该逻辑可防止短程攻击（例如，第3.4节中描述的贿赂攻击）。但是，它并不能阻止远程攻击：具有2/3投票权的验证者可以在所有资金解锁后密谋发布区块链分支。为了避免远程攻击，可以引入禁止远程分叉的机制（如在Nxt中）。

Slasher是由以太坊建筑师之一Vitalik Buterin概述的混合PoS / PoW算法。 与其他混合算法不同，Slasher专门使用工作证明来生成块; 每个块都使用PoW和PoS进行验证。

Casper是以太坊开发商Vlad Zamfir提出的赌注算法的概念证明。 与Tendermint类似，Casper使用块验证器的概念。 验证器通过为每个块分配概率来对块进行下注; 相同高度的块的概率总和必须等于100％。 为了在每个高度选择一个块，验证器可能需要执行几个下注轮次，直到至少2/3的验证器以高概率（例如，99％）在某个块上下注。 为了抵抗多数人的攻击，卡斯帕通过扣留一代奖励和锁定资金来自行为不当的验证人来惩罚偏离协议的行为。

纯粹的股权证明方法带来了巨大的安全威胁，无法在工作系统（包括比特币）的证明中重新创建。这些问题是股权算法证明所固有的，因为股权共识的证据并非固定在物理世界中。这就是为什么几乎所有依赖股权证明的货币都使用额外的机制来解决安全问题。


### 12. Bitcoin-NG: A Scalable Blockchain Protocol

**比特币NG：可扩展的区块链协议**

> 比特币衍生的区块链协议具有固有的可扩展性限制，在吞吐量和延迟之间进行权衡，这阻碍了这种潜力的实现。本文介绍了Bitcoin-NG（下一代），一种旨在扩展的新区块链协议。 Bitcoin-NG是一种拜占庭容错区块链协议，对极端流失很有效，并且与比特币共享相同的信任模型。除了比特币NG之外，我们还介绍了几种新的衡量标准，用于量化类比特币区块链协议的安全性和效率。我们实施比特币NG并以比例运营比特币系统15％的大小进行大规模实验，使用两种协议的未更改客户端。这些实验证明，比特币NG可以最佳地扩展，带宽仅受单个节点容量的限制，而延迟仅受网络传播时间的限制。

但区块链协议面临着显着的可扩展性障碍。这些系统处理事务的最大速率受到两个参数选择的限制：块大小和块间隔。增加块大小可以提高吞吐量，但是由此产生的更大的块需要更长的时间才能在网络中传播。减少阻塞间隔可以减少延迟，但会导致系统不一致并且区块链需要重组的不稳定性。

我们提出了基于与比特币相同的信任模型的可扩展区块链协议Bitcoin-NG。比特币NG的延迟仅受网络传播延迟的限制，其带宽仅受各个节点处理能力的限制。 Bitcoin-NG通过将比特币的区块链操作分解为两个平面来实现这种性能提升：领导者选举和交易序列化。它将时间划分为时代，每个时代都有一个单一的领导者。与比特币一样，领导者选举是随机进行的，很少进行。一旦选择了领导者，它就有权单方面地对交易进行序列化，直到选择了新的领导者，标志着前者的时代结束。

> 总之，本文做出了三点贡献。首先，它概述了Bitcoin-NG可扩展区块链协议，与比特币保持比特币信任假设相比，它实现了更高的吞吐量和更低的延迟。其次，它引入了评估Nakamoto共识协议的定量指标。这些指标旨在以比特币衍生货币的参数选择为基础进行讨论。最后，它通过大规模实验量化比特币NG的稳健性和可扩展性。

比特币-NG并没有引入自私采矿策略的新漏洞，因此比特币NG对于采用不到1/4采矿能力的攻击者进行自私采矿具有弹性。因此，我们认为比特币NG的保证在中本共识的有效性方面与比特币的保证相似。

> 双倍支出双重支出攻击仍然是比特币NG的一个漏洞，尽管程度低于比特币。


### [★] 13. Transactions as Proof-of-Stake

**交易作为股权证明**

> 利益证明背后的概念是一个区块链应该由链中有经济利益的人保护。 本文将介绍一种新的利益证明方法，利用每笔交易的硬币销毁日来代替目前工作证明所提供的绝大多数安全性。 与之前只有一些节点有助于股权证明计算的现有Proof-of-Stake系统不同，我们提出了一种新的利益证明方法，其中所有生成交易的节点都有助于网络的安全性。 我们推测这样一个网络对已知的比特币或Peercoin攻击免疫。

分散式系统面临的挑战是找到一种方法，每隔几分钟将广播限制为最多一个或两个节点。我们将提出一种不依赖于采矿的解决方案。

硬币日表示自特定硬币在网络上最后一次交易以来的天数。在任何给定的时间点，存在有限数量的硬币日，并且它们在长期持有大量余额的人手中累积。因此，硬币日可以被视为网络中股份的代理。每次涉及这些硬币的交易都会销毁硬币日，因此无法重复使用。

在本文中，我们提供了一种简化的Proof-of-Stake算法，该算法允许网络的所有用户为网络安全做出贡献以抵御攻击。对于任何行为者而言，维持一个包含比公共交易分类账更多的硬币日的秘密区块链在经济上是不可行的。所提出的技术解决了51％的攻击，自私采矿攻击，并提供防止双重支出的保护，同时根本不需要采矿。

由于股权证明可以消除对采矿奖励的需求，因此它们也消除了对通货膨胀的需求，同时也消除了浪费的能源消耗以进行工作量证明。在一个拥有越来越多的块链的世界中，通过工作量证明的安全性变得支离破碎而没有合并挖掘，并且合并挖掘有其自身的开销。通过这种新的合并证明方法，不再需要合并挖掘，并且可以支持无限数量的块链，而不会影响任何单个链的潜在安全性。


### 14. Anonymous Byzantine Consensus from Moderately-Hard Puzzles: A Model for Bitcoin

**来自中等难度谜题的匿名拜占庭共识：比特币模型**

> 我们提出了一个正式的同步过程模型，没有使用单向公共广播进行通信的不同标识符（即匿名进程）。 我们的主要贡献是证明比特币协议在此模型中达成共识，除了可忽略的概率，当拜占庭故障构成不到网络的一半时。 该协议是可扩展的，因为运行时间和消息复杂性都与网络的大小无关，而仅取决于故障进程的相对计算能力。 我们还要求协议必须容忍任意数量的接收广播但无法发送的被动客户端。 这导致紧密的2f + 1弹性界限。

Monte Carlo Consensus
> 我们在匿名对等网络模型中提出了比特币共识协议。 这样的协议可以实现全球事务处理器，广泛的公共网络，任何客户端将接收一致的视图，而不管它们的身份和它们在网络中的位置。 我们表明该协议符合其目标，至少在假设网络规模和通信延迟的知识时，以及大多数或进程正确执行协议时。 在未来的工作中，我们将尝试提高这种方法的可行性并避免这些假设。


### [★] 15. Casper the Friendly Finality Gadget

**Casper友好的终极小工具**

> 我们介绍了Casper，这是一个基于股权的终结系统的证明，它覆盖了现有的工作区块链证明。 Casper是一种结合利益算法研究证据和拜占庭容错共识理论的部分共识机制。 我们介绍我们的系统，证明一些理想的功能，并显示防范远程修订和灾难性崩溃。 Casper覆盖层几乎可以提供任何工作链证明，并具有针对块反转的额外保护。

PoS
> PoS设计有两个主要的思想流派。第一个基于链的股权证明，模仿工作机制的证明，并具有一系列区块，并通过伪随机分配向利益相关者创建新区块的权利来模拟挖掘。另一个流派是基于PoS的BFT共识算法。

Casper负责最终确定这些块，主要是选择一个代表分类帐规范交易的唯一链。 Casper提供安全性，但是活力取决于所选择的提议机制。 也就是说，如果攻击者完全控制提议机制，Casper可以防止最终确定两个冲突的检查点，但是攻击者可以阻止Casper完成任何未来的检查点。

> Casper引入了BFT算法不一定支持的几个新功能：
> 
> 问责制。如果验证者违反规则，我们可以检测到违规并知道哪个验证者违反了规则。问责制允许我们惩罚恶意验证者，解决困扰基于链的PoS的“无关紧要”问题。违反规则的处罚是验证人的全部存款。这种最大惩罚是防止违反协议。因为股权证券的证据是基于罚款的大小，其可以设定为大大超过采矿报酬的收益，所以股权证明提供了比工作证明更严格的安全激励.
> 
> 动态验证器。我们为验证器集引入一种安全的方式随时间变化.
> 
> 防御。我们引入针对远程修订攻击的防御以及超过1/3的验证器脱机的攻击，代价是非常弱的权衡同步性假设.
> 
> 模块化覆盖。 Casper的设计作为叠加层使其更容易实现，作为现有工作链证明的升级.

**卡斯帕的叉选择规则**
Casper比标准PoW设计更复杂。因此，必须调整前叉选择。我们修改后的fork-choice规则应该跟随所有用户，验证器，甚至底层块提议机制。如果用户，验证器或块提议者改为遵循“始终在最长链上建立”的标准PoW前叉选择规则，则存在Casper被“卡住”的病态场景，并且无法最终确定在最长链上构建的任何块（或者甚至是合理的）没有一些验证者利他主义地牺牲他们的存款。为了避免这种情况，我们引入一种新颖的，正确的构造，叉子选择规则：遵循包含最高高度的合理检查点的链条。这个分叉选择规则是正确的，因为它遵循合理的活动证明（定理2），它精确地说明总是可以在具有最大高度的合理检查点顶部完成新的检查点。此分叉选择规则将在第3节和第4节中进行调整。

结论
> 我们介绍了Casper，这是一种来自拜占庭容错文献的新颖的股权制度证明。 Casper包括：两个削减条件，一个受[8]启发的正确构造的叉子选择规则，以及动态验证器集。最后，我们介绍了Casper的扩展（不是还原最终检查点和不活动泄漏）来防御两种常见的攻击。
> 
卡斯珀仍然不完美。例如，完全受损的块提议机制将阻止Casper完成新块。 Casper是基于PoS的几乎所有PoW链的严格安全性改进。 Casper并未完全解决的问题，特别是与51％攻击相关的问题，仍然可以使用用户激活的软叉进行纠正。未来的发展无疑将提高Casper的安全性并减少对用户激活的软叉的需求。
>
未来的工作。当前的Casper系统建立在工作块提案机制的证明之上。我们希望将块提案机制转换为股权证明。即使验证器组的权重随奖励和处罚而变化，我们也希望证明其可靠的安全性和合理的活力。未来工作的另一个问题是对叉选择规则的正式规范，考虑到对股权证明的常见攻击。未来的工作报告将解释和分析卡斯珀的财务激励及其后果。与阻止攻击者的这种自动化策略相关的特定经济问题证明了不同客户端之间的不一致程度与攻击者所产生的成本之间的比率的上限。


### 16. Bitcoin: A Peer-to-Peer Electronic Cash System

**比特币：点对点电子现金系统**

> 纯粹的点对点电子现金版本允许在线支付直接从一方发送到另一方，而无需通过金融机构。数字签名提供了解决方案的一部分，但如果仍然需要受信任的第三方来防止双重支出，则主要优势将会丢失。我们提出使用点对点网络解决双重支出问题。网络时间戳通过将它们散列到正在进行的基于散列的工作证明链中进行交易，形成一条在不重做工作量证明的情况下无法更改的记录。最长的链不仅可以作为所见事件序列的证据，而且可以证明它来自最大的CPU功率池。只要大部分CPU功率由不协作攻击网络的节点控制，它们就会产生最长的链和外部攻击者。网络本身需要最小的结构。消息是在尽力而为的基础上广播的，节点可以随意离开并重新加入网络，接受最长的工作证明链作为它们消失时发生的事情的证据。

我们提出了一种不依赖信任的电子交易系统。我们从通常的数字签名框架开始，它提供了对所有权的强有力控制，但是如果没有防止双重支出的方法则是不完整的。为了解决这个问题，我们提出了一种使用工作量证明来记录事务公共历史的点对点网络，如果诚实节点控制大部分CPU能力，攻击者很快就会变得计算不切实际。该网络结构简单，结构简单。节点一次完成，几乎没有协调。它们不需要被识别，因为消息不会被路由到任何特定的地方，只需要尽力而为。节点可以随意离开并重新加入网络，接受工作证明链作为他们离开时发生的事情的证据。他们用他们的CPU权力进行投票，表达他们对有效块的接受，通过扩展它们并拒绝对它们进行处理来拒绝无效块。任何所需的规则和激励措施都可以通过这种共识机制来实施。


### [★] 17. Tendermint-  Consensus without Mining

**Tendermint-没有采矿的共识**

> 诸如比特币之类的加密货币使用户能够在不经过集中的可信组织的情况下提交支付交易。 比特币依赖于工作量证明挖掘来确保共识，这是有问题的; 采矿需要大量的能源消耗，交易确认缓慢，安全性难以量化。 我们提出了一种解决区块链共识问题的方法，该问题不需要通过调整现有解决方案来解决拜占庭常规问题。

我们的贡献是一种新颖的共识协议，它不需要工作量证明挖掘，并且具有高水平的防止双重攻击的保护。我们对参与者保持时间的能力做出了一个弱假设，我们假设网络的部分同步。我们的算法基于DLS协议的修改版本，并且可以恢复到1/3的拜占庭参与者。

理想的协议是激励兼容的纳什均衡，因此偏离协议不会导致净增益

结论
> Tendermint is awesome. The future is now.


### 18. PPCoin: Peer-to-Peer Crypto-Currency with Proof-of-Stake

**点点币：具有股权证明的点对点加密货币**

> 源自Satoshi Nakamoto的比特币的点对点加密货币设计。 股权证明取代了工作证明，以提供大部分网络安全性。 在这种混合设计下，工作证明主要提供初始铸造，从长远来看，这在很大程度上是不必要的。 从长远来看，网络的安全级别不依赖于能源消耗，因此提供了节能且更具成本竞争力的点对点加密货币。 利益证明基于硬币年龄，并且由每个节点通过与比特币相似但在有限搜索空间上具有相似性的散列方案生成。 区块链历史和交易结算受到中央广播检查点机制的进一步保护。

我们已经正式设计了一种共识机制，其中使用了利益证明来构建点对点加密货币的安全模型及其铸造过程的一部分，而工作量证明主要促进了铸造过程的初始部分。 并逐渐降低其意义。 该设计试图证明未来的点对点加密货币的可行性，而不依赖于能源消耗。 我们已将该项目命名为ppcoin。

> 币龄：简单地定义为货币金额乘以持有期。 在一个简单易懂的例子中，如果Bob从Alice收到10个硬币并持有它90天，我们就说Bob已经累积了900个硬币日的硬币年龄。

为了便于计算硬币年龄，我们在每个事务中引入了一个时间戳字段。 加强块时间戳和事务时间戳相关协议以确保硬币年龄的计算。

利益证明下的块生成在我们的混合设计中，块被分为两种不同的类型，即工作量证明块和证据块。

结论
> 在市场验证我们的设计后，由于消除了对能源消耗的依赖，我们希望利益证明设计成为可能更具竞争力的点对点加密货币到工作量证明设计形式， 从而在可比的网络安全级别实现更低的通货膨胀/更低的交易费.


### 19. The Byzantine Generals Problem

**拜占庭将军的问题**

> 可靠的计算机系统必须处理故障组件，这些组件会向系统的不同部分提供冲突的信息。这种情况可以用一群拜占庭军队的将军抽象地表达出来，他们的军队在敌人的城市周围扎营。将军通过信使进行沟通，必须就共同的战斗计划达成一致。但是，他们中的一个或多个可能是试图混淆其他人的叛徒。问题是找到一种算法来确保忠诚的将军达成协议。结果表明，只使用口头信息，当且仅当超过三分之二的将军忠诚时，这个问题才是可以解决的;所以一个叛徒可以混淆两个忠诚的将军。对于不可伪造的书面信息，任何数量的将军和可能的叛徒都可以解决这个问题。然后讨论解决方案在可靠计算机系统中的应用。

鲁棒性
> 鲁棒是Robust的音译，也就是健壮和强壮的意思。 它是在异常和危险情况下系统生存的关键。 比如说，计算机软件在输入错误、磁盘故障、网络过载或有意攻击情况下，能否不死机、不崩溃，就是该软件的鲁棒性。

拜占庭将军问题似乎看似简单。它的困难表现在一个令人惊讶的事实上，即如果将军只能发送口头信息，那么除非超过三分之二的将军忠诚，否则没有解决方案可行。

结论
> 我们在各种假设下提出了拜占庭将军问题的几种解决方案，并展示了如何将它们用于实施可靠的计算机系统。这些解决方案在时间量和所需消息数量方面都很昂贵。算法OM（m）和SM（m）都需要长度达到m 4- 1的消息路径。换句话说，每个中尉可能必须等待来自指挥官的消息，然后通过m个其他中尉进行中继。 Fischer和Lynch已经证明，任何可以应对m叛徒的解决方案都必须如此，因此我们的解决方案在这方面是最佳的。我们对未完全连接的图的算法需要长度达到rn + d的消息路径，其中d是忠诚将军的子图的直径。我们怀疑这也是最佳的。
> 
算法OM（m）和SM（m）涉及发送最多（n-1）（n-2）...（n-m-1）个消息。通过组合消息肯定可以减少所需的单独消息的数量。也可以减少传输的信息量，但是尚未对此进行详细研究。但是，我们希望仍然需要大量的消息。在任意故障面前实现可靠性是一个难题，其解决方案似乎本来就很昂贵。降低成本的唯一方法是对可能发生的故障类型做出假设。例如，通常假设计算机可能无法响应但永远不会错误地响应。然而，当需要极高的可靠性时，不能做出这样的假设，并且需要拜占庭将军解决方案的全部费用。


### [★] 20. A Simpleand Efficient Randomized Byzantine Agreement Algorithm

**简单有效的随机拜占庭协议算法**

> 本文提出了一种新的随机拜占庭协议算法。 该算法在n个处理器的同步系统中运行，其中至多t个处理器可能失败。 该算法在0（t / log n）预期轮次和O（n2tf / log n）预期消息比特中达成一致，而与处理器故障的分布无关。 如果假设处理器故障的分布是均匀的，则该性能进一步提高到恒定的预期轮数和O（n2）消息比特。 在任何一种情况下，该算法都针对确定性算法的轮数的已知下界进行了改进。 该算法的一些其他优点是它不需要加密技术，本地计算量很小，并且每个处理器使用的预期随机比特数只有一个。 有人认为，在拜占庭协议的许多实际应用中，本文的随机算法实现了优越的性能。


### 21. Comparative analysis of blockchain consensus algorithms

**区块链一致性算法的比较分析**

> 加密货币已经大受欢迎，这些新的虚拟货币背后是一种称为区块链的创新技术：一种分布式数字分类账，其中加密货币交易在经过验证后被记录。分类账中的交易由加密货币的对等网络内的多个客户或“验证器”使用许多不同的一致性算法之一来验证，以解决涉及多个不可靠节点的网络中的可靠性问题。最广泛使用的一致性算法是工作证明（PoW）算法和证明（PoS）算法；然而，还有其他一致的算法利用PoW和PoS的替代实现，以及其他混合实现和一些新的共识策略。在本文中，我们对典型的共识算法和当前在现代区块链中使用的一些同时代的算法进行了比较分析。我们的分析侧重于每个一致性算法所采用的算法步骤，算法的可扩展性，算法奖励验证器用于验证块的时间以及算法中存在的安全风险的方法。最后，我们提出了我们的结论和区块链中使用的一致性算法的一些可能的未来趋势。

### [★] 22. Proof of Vote: A High-Performance Consensus Protocol Based on Vote Mechanism & Consortium Blockchain

**投票证明：基于投票机制和联盟区块链的高绩效共识协议**

> 比特币引入了革命性的分散共识机制。 然而，应用于公共区块链的比特币衍生共识机制不适用于新兴财团区块链的部署方案。 我们提出了一种新的共识算法，即投票证明（POV）。 共识由财团合作伙伴控制的分布式节点协调，这些节点将通过投票进行分散仲裁。 关键的想法是为网络参与者建立不同的安全身份，这样块的提交和验证是由联盟机构在联盟中的投票决定的，而不依赖于第三方中介或无法控制的公众意识。 与完全分散的共识工作证明（POW）相比，POV具有可控的安全性，收敛可靠性，只有一个块确认才能实现事务的最终性，以及低延迟的事务验证时间。

POV，一种基于投票机制和联盟区块链的共识协议。

由于块生产所消耗的大量时间和能量以及安全性能，目前为区块链设计的共识机制很慢。提供了对共识算法的不同折衷作为权衡以实现分布式系统中的一致性。一种方法是划分计算能力，例如比特币和以太坊所代表的工作证明（POW）。另一种方法是依靠代币，例如由Peercoin代表的证明（POS）和由Bitshare代表的代理证明（DPOS）。除了这些不可避免的折扣之外，由于存在分叉的可能性，现有解决方案仍然难以在安全要求下加速交易确认。亚瑟等人，分析了POW的安全性，发现比特币最突出的分支Litecoin和Dogecoin将块生成间隔从10减少到2.5和1分钟。但是，它们仍需要28和47个块确认才能匹配比特币的安全性，从而导致高延迟事务验证。然而，本文提出的POV巧妙地利用了联合体区块链的特征。通过投票结果最终生成唯一的有效块，从而优化交易确认时间和系统的高吞吐量。

在本文中，我们提出了POV的完整共识过程。在POV中，成员节点具有投票权，具有高投票权的块是vaild，使得有效块唯一。一些特殊节点为了生成块而运行，以便在联盟区块链网络中直接进行交易而无需任何第三方中介。我们分析安全性，交易终结性和分叉的可能性。如本文所示，POV可以在事务验证中获得极佳的性能和超低延迟。

POV共识过程中有以下四个角色：委员，管家，管家候选人和普通用户。

有两个主要的投票程序。第一个是对块生产的投票，第二个是对管家候选人的投票。委员们通过返回他们的签名进行投票。

结论
> 在本文中，我们提出了一种新的共识机制（POV），专门用于联盟区块链。 我们根据投票活动和投票机制的关键思想为网络参与者设计了四个身份。 前者保证了投票权与行政权的分离，增强了投票者角色的独立性，财团内部控制系统也是如此。 至于后者，在至少Nc / 2 + 1专员有效工作的情况下，我们的分析表明POV可以保证安全性，交易最终性，低功耗并确保区块链永远不会分叉。 我们通过参数调整进一步分析了POV的可靠性，并证明了其在低事务延迟方面的强大性能。


### 23. Zero-determinant strategy for the algorithm optimize of blockchain PoW consensus

**区间链PoW共识算法优化的零决策策略**

> 工作证明（PoW）一致性算法保证了区块链系统的安全性和可靠性。 在采矿过程中，矿工可以通过PoW算法达成共识，即相互攻击。 然而，当矿工互相攻击时，所有矿工的收入都会减少。 在本文中，我们建立了一个模型，两个矿工之间的挖掘是一个迭代游戏，并提出了一个ZD策略的子类（一个缓解策略），以减轻矿工的困境，矿工可以控制另一个矿工的收益，并通过一个增加社会收入 钉住策略。 数值仿真结果验证了该策略的有效性。 总之，这项工作通过博弈论可以更好地理解和分析PoW算法，从而有可能在未来设计更合理的一致性算法。

PoW共识机制旨在确保比特币分布式会计系统的一致性。不幸的是，它也有许多缺点。有一些改进的共识算法，如股权证明（PoS），它将PoW的权力变为系统权利，更大的玩家所有权更有可能成为下一个账户。 PoS既节能又节省时间，但它很容易上叉，也需要开采。委托证明（DPoS）取决于PoS扮演会计专业人员的角色，其中帐户由权利选择的玩家保存。它显着减少了身份验证和记帐所涉及的节点数量，并达到了共识验证的第二级。而它仍然依赖于令牌。基于传统分布共识技术的验证池[16]使用数据验证机制。它没有令牌，保持低度的偏心。委托拜占庭容错算法选择由权利选择的簿记员来达成共识，这最大化了系统的完整性，但也分散了很多。目前的共识机制都不是完美的或适用于所有应用场景。

结论
> 在本文中，我们分析了矿工在PoW共识过程中的困境，并通过博弈论优化了PoW共识。 为了防止两个矿工互相攻击，我们提出了一个钉扎策略，一个ZD战略的子类，它可以设定SM的收益，从而提高社会收入。模拟结果证实，当LM采用钉扎策略时，比特币系统 无论SM的战略如何，都获得相对较高的社会收入。 此外，我们已经证明LM无法用任何策略控制自己的收益。
> 
基于钉扎策略的分析，我们发现SM的收益与r成正比，但与c成反比。 因此，为了提高SM合作的可能性并增加社会收入，可以通过提高r的值或降低c的值或应用钉扎策略来优化区块链系统。


### [★综述] 24. A review on consensus algorithm of blockchain

**区块链一致性算法综述**

> 区块链是比特币的基本技术。 随着比特币的价值增值和稳定运行，区块链在许多领域受到越来越多的关注。 区块链具有分散，稳定，安全和不可修改的特征。 它有可能改变网络架构。 共识算法在维持区块链的安全性和效率方面起着至关重要的作用。 使用正确的算法可以显着提高区块链应用程序的性能。 在本文中，我们回顾了共识算法的基本原理和特征，并分析了不同共识机制的性能和应用场景。 我们还提供了选择合适的一致性算法的技术指导，并总结了区块链技术的局限性和未来发展。

**区块链技术包括点对点（P2P）通信，一致性算法，分布式存储技术，加密算法等。** 但目前，区块链的研究主要集中在比特币或区块链在不同领域的应用。 因此，在本文中，我们在第二章中介绍了现有的通用共识算法，并分析了共识算法的性能和缺点。 然后，我们在第三章中就如何在不同场景中选择合适的一致性算法给出了指导。

在区块链的应用中，我们需要解决两个问题双重花费和拜占庭将军问题。双重支出问题意味着同时在两个交易中重复使用货币。传统货币是实体，因此我们不会在使用传统货币时面临双重支出的问题。我们还可以通过集中的可信机构解决互联网交易中的双重支出问题。 Blockchain通过将许多分布式节点一起验证事务的方法解决了这个问题。拜占庭将军问题是分布式系统中的问题。可以通过对等通信在不同节点之间传递数据。但是，某些节点可能受到恶意攻击，这将导致通信内容的变化。普通节点需要区分已被篡改的信息并获得与其他正常节点一致的结果。这也需要相应的一致性算法的设计。

PoW
> PoW是比特币中使用的一致性算法。其核心思想是通过节点之间的散列功率竞争来分配会计权利和奖励。基于前一个块的信息，不同的节点计算数学问题的具体解。解决数学问题很困难。解决此数学问题的第一个节点可以创建下一个块并获得一定数量的比特币奖励。 Satoshi Nakamoto使用HashCash在比特币中设计这个数学问题。具体计算步骤如下：
> 
- 获取难度：每生成2016块后，比特币挖掘算法将根据整个网络的哈希率动态调整难度值。
- 收集事务：在生成最后一个块之后收集网络上的所有待处理事务。然后计算这些事务的Merkle Root并填写块版本号，前一个块的256位哈希值，当前目标哈希值，Nonce随机数和其他信息。
- 计算：将Nonce从0移动到232并在步骤2中计算双SHA256哈希值。如果哈希值小于或等于目标值，则可以广播该块。节点完成计费后验证其他节点。
- 重新启动：如果节点在某个时间无法计算出哈希值，则重复第二步。如果任何其他节点完成计算，则从步骤1重新开始。
>
PoW将工作量作为安全措施。新创建的块链接到它前面的块。链的长度与工作量成比例。所有节点都信任最长的链。如果有人想要篡改区块链，他需要控制世界上50％以上的哈希能力，以确保他能够成为第一个产生最新区块并掌握最长链的人。篡改带来的收益远远大于成本。因此，PoW可以有效地保证区块链的安全性。

PoS
> 在PoS中，数字货币具有硬币年龄的概念。硬币的硬币年龄是它的值乘以它创建后的时间段。一个节点持有硬币的时间越长，它在网络中获得的权利就越多。根据硬币年龄，硬币的持有者也将获得一定的奖励。在PPCoin的设计中，还需要采矿来获得会计权利。公式是证明<硬币年龄*目标。校对是权重因子的组合哈希值，未使用的输出值和当前时间的模糊和。 PoS限制每个节点的散列功率。采矿的难度与硬币年龄成反比。
> 
PoS鼓励硬币持有者增加持有时间。随着硬币时代的概念，区块链不再完全依赖于工作证明。这有效地解决了PoW中的资源浪费问题。使用PoS的区块链的安全性随着区块链中的价值增加而提高。攻击者需要积累大量硬币并将其保持足够长时间以攻击区块链。这也大大增加了攻击的难度。
>
除了PPCoin之外，还有许多使用PoS的硬币，如Nxt和BlackCion。但他们考虑节点的权利，并使用随机算法来分配会计权利。

DPoS(Delegated Proof of Stake)
> BitShares是DPoS的一个例子。在具有DPoS的区块链中，每个节点可以根据其赌注选择证人。在整个网络中，参与竞选并获得最多选票的前N名证人拥有会计权。确定证人数量N，使至少50％的投票利益相关者认为有足够的权力下放。当选的证人一个接一个地创建新的区块并获得一些奖励。证人需要确保足够的在线时间。如果证人无法创建其指定的区块，则该区块的活动将移至下一个区块，利益相关者将投票选择新的证人进行替换。使用DPoS的区块链比PoW和PoS更高效，更省电。

PBFT(Practical Byzantine Fault Tolerance)
> 在分布式系统中，拜占庭容错可以是解决传输错误的好方法。但早期的拜占庭系统需要指数运算。直到1999年，提出了PBFT（实际拜占庭容错）系统，并将算法复杂度降低到多项式水平，大大提高了效率。 PBFT的过程如图1所示。它由五种状态组成：
> 
- 请求：客户端向主服务器节点发送请求，主节点向请求提供时间戳。
- 预备：主服务器节点记录请求消息并为其提供订单号。然后，主节点向其他服务器节点广播预准备消息。其他服务器节点最初确定是否接受请求。
- 准备：如果服务器节点选择接受请求，它将向所有其他服务器节点广播准备消息，并从其他节点接收准备消息。收集2f + 1消息后，如果大多数节点选择接受请求，则它将进入提交状态。
- Commit：处于提交状态的每个节点都向服务器中的所有其他节点发送提交消息。同时，如果服务器节点收到2f + 1个提交消息，则可以认为大多数节点达成共识以接受该请求。然后，节点执行请求消息中的指令。
- 回复：服务器节点回复客户端。如果客户端由于网络延迟而未收到回复，则会将请求重新发送到服务器节点。如果请求已执行，则服务器节点只需重复发送回复消息。

Raft
> 在提出拜占庭将军问题之后，Lamport提出了Paxos算法来解决1990年某些条件下的一致性问题。

> Raft集群通常包含5个服务器节点。允许最多两个节点同时崩溃。如图2所示的服务器节点有三种状态：leader，follower和candidate。一个学期只有一个领导者，领导者负责处理所有客户的请求。

共识算法分析
> 所有共识算法都有自己的特点。 在本章中，我们分析了安全性，验证速度，吞吐量（每秒事务数，TPS），容错性，可扩展性以及共识算法的缺点以及在不同场景中的使用。

> 为了减少分叉并等待足够的块来确认，使用PoW或PoS的区块链的吞吐量是有限的。在这个区块链中，所有节点都可以根据预先设定的规则进行挖掘。吞吐量和验证速度与节点数无关。因此，这种区块链网络具有几乎无限的可扩展性。
> 
在使用DPoS的区块链中，当选的证人负责创建区块和确认交易。为了减少验证节点，使用DPoS的区块链可以加快创建块和验证事务的速度。 DPoS的吞吐量和事务验证速度比PoW或PoS快。可扩展性也是无限的。

>
使用PBFT的区块链由3f + 1个服务器节点组成，每个节点需要在通信中收集2f + 1个消息。因此，这种区块链系统可以容忍最多33％的恶意节点。 PBFT还包含视图更改机制。视图更改机制是在主节点出错或系统无法长时间完成客户端请求时用以下节点替换主节点。由于PBFT中的节点需要与每个节点通信以达成协议，因此可扩展性受到限制。 PBFT更适用于具有高速网络和少量节点的许可区块链系统。

>
Raft具有高效率和简单性，并且已广泛用于分布式系统中。在RAFT区块链中，领导者占据绝对优势地位。区块链不能容忍恶意节点，并且可以容忍高达50％的崩溃故障节点。保证领导节点的绝对安全性非常重要。吞吐量受到一个节点的最大性能的限制。可扩展性受RAFT架构的限制。


### 25. PoPF: A Consensus Algorithm for JCLedger

**PoPF：JCLedger的共识算法**

> JointCloud是新一代云计算模型，可以帮助开发人员定制云服务。JCLedger是一种基于区块链的联合云计算分布式账本，可以使云资源交换更加可靠和方便，是JointCloud和BlockChain的结合。创建JCLedger最重要的元素之一是一致性算法。PoW（工作证明）是比特币的一致性算法，它被证明是非常安全的，但需要很大的计算能力。原始PoW不适合JCLedger，因为参与者的身份在计算能力上不相等，这可能导致会计垄断，并且吞吐量不能满足JointCloud中大规模和高频率交易的要求。在本文中，我们提出了一种基于PoW的共识算法，称为参与和费用证明（PoPF），它可以为JCLedger节省大量计算能力并更有效地处理事务。在我们的设计中，只有候选人有机会进行挖掘，并根据排名选择候选人，排名由两个因素决定：参与者作为会计师的时间和参与者支付的费用。解决PoW哈希拼图的候选人的难度是不同的（较高的排名意味着更容易挖掘）。仿真实验表明，会计师的分布很均衡，也就是说，JointCloud中参与者的不等计算能力得到了屏蔽，所有在JCLedger中有足够贡献的用户都有机会成为会计师。

在本文中，我们提出了一种基于PoW的JCLedger一致性算法，它可以避免计算能力的巨大成本，屏蔽参与者的不等计算能力，给予他们平等的会计机会。处理JCCE中的大规模和高频交易比原始PoW更有效。

PoPF
> 该方法的名称称为参与证明和费用。我们根据用户参与（会计时间）和先前交易中的费用（用户支付的费用）确定的排名选择每个区块的会计候选人。排名前n％的用户是会计候选人。他们通过解决哈希拼图来竞争包装下一个块的权利，这与比特币系统中的PoW挖掘相同。然而，不同之处在于每个用户的挖掘难度并不相同，与排名较低的用户相比，更高级别的用户更容易赢得竞争。总之，系统根据参与和费用为不同的用户设置不同的挖掘难度􏰁这就是算法被称为PoPF的原因。


### 26. A Proof-of-Trust Consensus Protocol for Enhancing Accountability in Crowdsourcing Services

**加强众包服务问责制的信任证明共识议定书**

> 将问责机制纳入在线服务需要有效的信任管理和交易证据的不可改变的，可追溯的事实来源。区块链技术的出现带来了很大的希望，以满足大多数这些要求。然而，一个主要挑战是找到适用于特别是众包服务和一般在线服务的适当共识协议。在利用区块链作为支持服务合同和争议仲裁的跟踪交易的基础技术的基础上，本文提出了一种适用于众包以及一般在线服务行业的新型共识协议。新的共识协议被称为“信任证明”（PoT）共识；它根据服务参与者的信任值选择交易验证人，同时利用Raft领导者选举和Shamir的秘密共享算法。PoT协议避免了与比特币的“工作证明”（PoW）挖掘相关的低吞吐量和资源密集缺陷，同时解决了与传统的基于Paxos和拜占庭故障容忍（BFT）的算法相关的可扩展性问题。此外，它还解决了传统BFT算法无法解决的不忠行为。该论文表明，我们的方法可以为在线服务行业提供可行的问责解决方案。

因此，我们概述了实现服务责任的此类责任的基本要求。
>
要求1：基础设施必须在一定程度上分散，不存在单独的集中授权，因为集中授权在可扩展性，安全性，公平性和客观性方面有明显的局限性;
>
要求2：服务合同应对所有服务参与者公开显示。 必须明确规定义务和相关的服务活动;
>
要求3：签约方合同执行期间应有一个共同的，不可变的服务活动日志; 
>
要求4：应该有一个仲裁机制来解决服务提供商和消费者之间的争议。仲裁机制应该是无党派和公平的，但它需要在保持诚实仲裁者的同时提供激励整体仲裁成本低。
>
要求5：共识协议必须能够提供低延迟和高吞吐量;
>
需求6：基础设施应该支持数百万参与者;
>
要求7：共识协议应该在开放的环境中管理不忠和拜占庭的错误;
>
要求8：共识过程应该是公正和公平的。

分布式共识

>
1982年，Lamport发表了他的开创性论文“拜占庭将军问题”。在他的论文中，Lamport证明了在同步通信的条件下，必须至少有3f + 1个节点才能达到非故障节点的共识，最多只有f“拜占庭”故障节点。与不影响系统其余部分的所谓“崩溃恢复”故障形成对比，“拜占庭”故障意味着即使节点出现任意且不一致的行为，它也可能继续与系统的其余部分进行交互，或串通以设计更多的恶意输出。
>
在消息延迟不受限制的异步环境中，无法找到能够同时保证协议有效性和活性的共识协议。
>
解决“拜占庭”故障的第一个共识协议是Castro和Liskov在1999年提出的实用拜占庭容错（PBFT）协议。 PBFT在通信异步的环境中实现了共识，但是消息延迟是有限的，并且最多f <n / 3的服务器是拜占庭服务器。
>
**其他BFT容忍共识协议，如Zyzzyva，FaB Paxos，XFS，对可以容忍的拜占庭节点数量以及通信效率提供了不同的权衡。但总的来说，基于BFT的共识协议适用于小规模的状态机复制方案。**
>
另一种共识协议基于Lamport在中提出的Paxos。 Paxos是一种确定性算法，可在异步系统中运行，并且可以容忍f <n / 2“崩溃恢复”故障，其中f是故障节点的数量。 Paxos牺牲终止的正确性，即协议和有效性属性。但是，通过简单地设置更长的超时值，可以在实践中应用该协议。 Paxos协议激发了研究人员开发许多Paxos，如共识协议，如Google的Chubby，Yahoo的Zookeeper，etcd，Raft等。
>
Paxos协议的问题在于难以理解和实现。而Raft的效率相当于Paxos，但它比Paxos具有更易理解的结构，也为构建实用系统提供了更好的基础。为了提高可理解性，Raft将共识的关键要素（如领导者选举，日志复制和安全性）分开，并强制实施更强的一致性，以减少必须考虑的状态数量。

虽然以上三类共识算法可以解决PoW的缺点，但它们都有自己的弱点，总结如下：

> “股权证明”一般遭受“无利害关系“，其中块生成器通过投票选择多个区块链历史而没有任何损失，这导致共识永远不会解决。由于在几个连锁店工作时缺乏成本障碍，情况更加恶化。 PoS的另一个缺点是它缺乏“公平性”，因为最富有的参与者总是被给予最简单的挖掘难题。

> 基于Paxos的共识和拜占庭容错（BFT）算法通常缺乏可扩展性，因此它们仅适用于小规模分布式环境。当参与者节点的数量增加时，共识过程的性能将呈指数级降低。

共识流程描述：

> 阶段1 - 分类账管理的领导者选举

> 阶段2 - 分类帐管理负责人指定服务交易验证组

> 阶段3 - 事务验证组成员对应填写下一个块的事务进行投票

> 阶段4 - 分类账管理投票和簿记

协议分析
我们总体上基于有效性，一致性，活跃性，性能，可扩展性，公平性和安全性来分析PoT共识协议。 我们还讨论了许多可能的攻击情形。


### [★] 27. Proof of Contribution: A Modification of Proof of Work to Increase Mining Efficiency

**贡献证明：提高采矿效率的工作证明修改**

> 基于工作证明的区块链浪费了大量电力，需要昂贵的采矿设备。 这种现象越来越严重。 我们提出了一种新的基于比特币协议的加密货币共识协议，它将工作证明组件与我们新的算法证明（PoC）相结合。 PoC算法通过奖励加密拼图的计算难度来降低比特币挖掘的能耗。 此外，当矿工不再获得集体奖励时，他们会收到困难的奖励以及促使采矿的常规采矿费。 我们探讨了不同的攻击场景，并表明对这些攻击具有弹性的网络与Poof-of-Work（PoW）相当。 最后，我们设计了两个实验来模拟挖掘并检测难度的变化，以证明PoC提供了一种新的加密货币算法，该算法具有高能效。

在基于PoS的算法中，通过随机选择与“桩”的各种组合来实现分布式共识。参与者对区块有效性的投票权取决于他们的利益。赌注的形式在不同的实施方式中有所不同。 Peercoin使用“造币”作为铸造新币的赌注。造币是通过将硬币数量与其持有的天数相乘得出的。一旦硬币的桩子用于铸造新硬币，他们的硬币将被重置为零。最大铆接年龄设定为90天，以防止极其古老的硬币占主导地位。Tendermint使用拜占庭问题的解决方案来达成共识。根据Tendermint协议，验证人是通过债券交易锁定其硬币的用户。他们的投票权与他们锁定的硬币数量有关。这些算法试图在没有大量计算能力的情况下达成共识。然而，基于PoS的算法存在若干新问题。例如，当用户对所有分叉进行投票以获得最大利益并且它不是完全分散的解决方案时，就会出现“无利害关系”问题。

为了解决高能耗问题，我们提出了一种新的共识算法，称为分布证明（PoC）。与Peercoins的一致性算法类似，我们的算法结合了PoW和PoS。通过算法的PoS组件实现能量效率。与Peercoin中的造币相比，赌注是基于矿工的诚实。它计算为矿工将有效区块添加到区块链的次数，表示为成功时间。成功时间系数决定了矿工的采矿难度。每个矿工都有不同的难度级别。矿工成功时间越高，越容易开采。 PoC不是单独依靠散列能力来获得更高的采矿区块概率，而是通过与成功时间相结合来提高矿工找到区块的可能性。矿工可以通过查看区块链上的交易来验证其他矿工的成功时间和难度。矿工维护黑名单以阻止不当行为并使网络能够抵御攻击。作为对不当行为的惩罚，一旦其地址被列入黑名单，矿工的所有难度奖励都将被撤销。 PoC激励诚实行为，同时劝阻不当行为。但是，没有讨论黑名单的重要方面，例如，如何定义不当行为以及如何检测攻击。

这项工作的主要贡献是我们提出了新的一致性算法，它减轻了高能耗，提高了比特币网络的挖掘效率。

PoC通过引入成功时间来扩展PoW，这是一种调整矿工采矿难度的机制。 PoC保持了与工作证明相同的难度调整机制。如果网络难度降低，协议将降低难度以确保相同的平均交易时间。由于PoC的主要变化是调整矿工的采矿难度，因此在真实的比特币网络中实施修改将很容易。由于不同的矿工有不同的成功时间，因此根据矿工的成功时间c，引入难度因子β来调整矿工的难度。

为了解决更高计算要求的问题，我们提出了一种名为“贡献证明”的新算法，该算法基于工作量证明和证据证明。员工的诚实表现为成功时间被用作“赌注”来调整PoC挖掘过程中的难度。 PoC算法对诚实的矿工友好，并惩罚恶意行为。实验表明，在相同的计算情况下，PoC中的全局难度会更快。换句话说，随着网络的增长，添加新散列功率的成本也会增加。它鼓励矿工诚实，避免不良行为，而不是购买更多的机器。它是通过集成PoS组件实现的，称为成功时间。


### 28. Delegated Proof of Stake: Features & Tradeoffs

**委托的股权证明：特征和权衡**

委托证明（DPoS）将块生产集中在少数已知的半可信实体中，比工作量证明（PoW）或其他证据证明具有更高的可扩展性数量级（PoS）区块链。 

在DPoS中，持有网络令牌的人能够投票选举区块生产者；投票由选民的赌注加权，获得最多选票的区块制作人候选人是那些产生区块的人。用户还可以将他们的投票权委托（“代理”）给可以代表他们投票的其他用户。

DPoS允许用户投票与他们的赌注成比例，以决定谁产生积木。大块生产者本身不一定需要拥有大量股份，但他们必须竞争以获得用户的投票。

DPoS的一个有趣特征是，当块生产者候选人竞争令牌持有者投票时，选举的块生产者实际上合作以在轮次期间保护网络。区块生产者平等地分享区块奖励（来自通货膨胀），并且它们每轮只能产生一个区块。由于这是不可能的，因此没有激励块生产者竞争试图生产比其他生产者更多的块。

DPoS存在一些缺点，主要是它对令牌持有者提出了更多要求，以监控网络的健康状况，注意不良行为，并决定什么能够实现充分的分散。然而，作为交换，DPoS提供了巨大的性能增强，并具有其他非常有利的属性。我们相信DPoS具有非常引人注目的功能和权衡，使其成为许多类型的分散应用程序的理想解决方案。

DPoS认识到权力下放在经济和性能方面都具有成本，并且它选择半集中化来换取可扩展性。如果DPoS系统仍然可以提供必要级别的审查阻力，无权限和无信任，那么DPoS对于大量分散应用程序更好。对于某些用例绝对具有审查能力的数字黄金，点对点数字货币等，在牺牲性能的情况下支持权力下放的权衡可能是有意义的。对于绝大多数应用程序而言，可伸缩性更加实用。


### 29. Fast Byzantine Consensus

**快速的拜占庭共识**

> 我们提出了第一个在常见情况下在两个通信步骤中达到异步拜占庭共识的协议。 我们证明我们的协议在通信步骤的数量和两步共识的过程数量方面是最佳的。 该协议可用于构建复制状态机，在常见情况下每个请求仅需要三个通信步骤。 此外，我们展示了协议的参数化版本，尽管f拜占庭故障是安全的，并且在通常情况下保证两步执行，尽管有一些故障数t（t≤f）。 我们表明，这种参数化的两步共识协议在通信步骤数和进程数方面也是最优的。

共识问题可以用三类代理人采取的行动来描述：提议者，提出价值观，接受者，共同负责选择单一建议价值的人，以及必须学习所选价值的学习者。

Paxos
> 自从简单实用的Paxos协议的发掘以来，多年来一直是理论论文焦点的共识再次受到从业者的欢迎。鉴于共识是状态机方法的核心，这是在分布式系统中实现容错服务的最常用方法，因此这种受欢迎程度应该不足为奇。然而，许多从业者对于在一个错误的过程中在异步系统中确定性地解决共识的可证明的不可靠性感到沮丧。 Paxos提供了下一个最好的东西：尽管它不能保证某些情况下的进展，但它总是保留了共识的安全属性，尽管异步和进程崩溃。更具体地说，在Paxos中，其中一位提议者被选为领导者，负责与接受者沟通。 Paxos只有在领导者独特并且能够及时与足够多的接受者沟通时才能保证进步，但即使没有领导者或多个领导者也能确保安全。我们的协议遵循类似的结构，但我们从提议者而不是接受者中选择领导者。
> 
Paxos也很有吸引力，因为它可以在优雅的执行中非常有效，即（i）有一个独特的正确领导者，（ii）所有正确的接受者就其身份达成一致，以及（iii）系统处于以下期间的执行：同步。请注意，在领导执行期间，领导者以外的流程可能仍会失败。除了在病理情况下，有理由期望优雅的执行将成为常态，因此需要对它们进行优化。例如，Boichat等人的FastPaxos协议。只需要两个沟通步骤1，以便在非拜占庭环境中达成共识，匹配由Keidar和Rajsbaum形式化的下限（FastPaxos不应该与Lamport最近的“Fast Paxos”（带空格）相混淆使用不同的方法来减少常见情况下的通信步骤数量。因此，在使用FastPaxos的状态机中，一旦领导者收到客户端请求，在通常情况下，在执行请求之前只需要两个通信步骤。从此以后，我们可以互换地使用“普通案例”和“亲切执行”这两个术语。

快速拜占庭（或FaB）Paxos，一种拜占庭共识协议，在常见情况下完成两个通信步骤（我们说它是两步），而不使用昂贵的数字签名。 FaB Paxos需要5f + 1个受体并且能够容忍f拜占庭故障。其次，我们展示了FaB Paxos参数化FaB Paxos的推广 - 它需要3f + 2t + 1个受体来容忍f拜占庭失败，并且只要最多t个受体失败就是两步。

FaB Paxos在常见情况下不使用数字签名;但是，在选举新领导者时，它确实依赖于数字签名。所有接受者都有公钥/私钥对 - 我们假设所有提议者和接受者都知道所有公钥，并且正确的接受者不会泄露他们的私钥。我们还假设拜占庭进程无法破坏加密原语。由于在异步模型中不可能同时提供安全性和活跃性[5]，我们始终确保安全，并且只保证在同步期间的活跃度。

FaB
> 我们现在介绍FaB Paxos，这是一个两步拜占庭容错共识协议，需要5f + 1个过程 - 在第VI节中，我们表明这个数字是最优的。 更确切地说，FaB Paxos需要≥5f+ 1个受体，p≥3f+1提议者和l≥3f+1个学习者; 与Paxos一样，FaB Paxos中的每个流程都可以扮演这三个角色中的一个或多个角色。 我们分阶段描述FaB Paxos：我们首先描述一个依赖于相对较强的假设的协议的简单版本，然后我们逐步削弱假设并完善协议。

我们的端到端重传策略基于以下模式：调用者重复发送其请求，并且每次收到请求时被调用者都会发送一个响应。当呼叫者对回复感到满意时，它将停止重新发送。我们稍微改变模式以适应领导者选举协议：其他过程必须能够确定领导者是否正在取得进展，因此领导者必须确保他们也接受回复。为此，学习者不仅要向领导者报告，还要向其他提议者报告。当提议者收到足够的确认时，他们会“满意”并通知领导者。领导者只有在收到⌈（p + f + 1）/2⌉这样的通知时才停止重发。如果提议者在一段时间后没有听到⌈（l + f + 1）/2⌉学习者的话，他们会开始怀疑领导者。如果⌈（p + f + 1）/2⌉提议者怀疑领导者，则选举新的领导者.5因此，转发政策确保在同步期间领导者将重新传输，直到确保不会触发领导者选举为止。请注意，提议者不要等到他们听到所有学习者之后才会感到满意（因为有些学习者可能已经崩溃）。因此，领导者可能在所有学习者已经学习了价值之前停止转发。为了确保最终所有正确的学习者都能学到价值，协议第30-42行要求所有正确的学习者仍然处于黑暗状态，以便从同龄人那里获取价值。

FaB Paxos是第一个在常见案例中仅通过两个沟通步骤达成共识的拜占庭共识协议。该协议是最佳的，因为它使用最少数量的步骤来达成共识，并且它使用最少数量的进程来确保在常见情况下的两步操作。此外，FaB Paxos在常见情况下不需要昂贵的数字签名。


### 30. Impossibility of Distributed Consensuswith One Faulty Process

**一个错误过程的分布式共识的不可能性**

> 共识问题涉及异步的过程系统，其中一些可能是不可靠的。问题在于可靠的处理是否同意二进制值。在本文中，表明即使只有一个错误的过程，这个问题的每个协议都有可能发生不确定性。

在本文中，我们展示了令人惊讶的结果，即没有完全异步的共识协议甚至可以容忍一个未公布的过程死亡。我们不考虑拜占庭式的失败，我们假设消息系统是可靠的，它可以正确而准确地传递所有消息一次。尽管如此，即使有了这些假设，单个进程停止运行的时间也会导致任何分布式提交协议无法达成一致。因此，如果没有关于计算环境的进一步假设或者对可容忍的故障类型的更大限制，这个重要问题就没有可靠的解决方案！

我们证明的关键是处理是完全异步的;也就是说，我们不会假设处理器的相对速度或传递消息的延迟时间。我们还假设这些进程没有访问同步时钟，因此不能使用基于超时的算法。最后，我们不假设检测过程死亡的能力，因此一个过程不可能判断另一个过程是否已经死亡（完全停止）或是只是跑得很慢。

我们已经表明，在完全异步的计算模型中无法解决容错协同计算的自然和重要问题。 这些结果并未表明这些问题在实践中无法“解决”; 相反，他们指出需要更精确的分布式计算模型，以更好地反映关于过程和通信时间的现实假设，以及对这些问题的解决方案的较低要求。（例如，可能只需要以概率1来终止终止。）在接下来的情况下，我们可以根据这些情况进行终止，为这些线路提供更多信息。


### 31. In Search of an Understandable Consensus Algorithm

**寻找可理解的共识算法**

> Raft是用于管理复制日志的一致性算法。 它产生的结果相当于（多）Paxos，它和Paxos一样有效，但它的结构与Paxos不同; 这使得Raft比Paxos更容易理解，也为构建实用系统提供了更好的基础。 为了提高可理解性，Raft将共识的关键要素（如领导者选举，日志复制和安全性）分开，并强制实施更强的一致性，以减少必须考虑的状态数量。 用户研究的结果表明，Raft比Paxos更容易学生学习。 Raft还包括一种用于更改群集成员资格的新机制，该机制使用重叠主要来保证安全性。

在设计Raft时，我们应用特定技术来提高可理解性，包括分解（Raft分离领导者选举，日志复制和安全性）和状态空间减少（相对于Paxos，Raft减少了不确定性的程度以及服务器可能与之不一致的方式）。

它有几个新颖的特征：
	
	* 强有力的领导者：Raft使用更强大的领导力
比其他共识算法。例如，日志条目仅从领导者流向其他服务器。这简化了复制日志的管理，使Raft更易于理解。
	
	* 领袖选举：Raft使用随机计时器来选举领导者。
这为任何共识算法已经需要的心跳添加了少量机制，同时简单快速地解决冲突。

	* 成员资格变化：Raft的机制改变了集群中的服务器集使用了一种新的联合共识方法，其中两种不同配置的多数在转换期间重叠。这允许群集在配置更改期间继续正常运行。
	
我们相信Raft优于Paxos和其他共识算法，无论是出于教育目的还是作为实施的基础。它比其他算法更简单，更易于理解；它的描述完全足以满足实际系统的需要;它有几个开源实现，并被几家公司使用;其安全性能已经过正式规定和验证；其效率与其他算法相当。

> 复制状态机用于解决分布式系统中的各种容错问题,通常使用复制日志实现。

当领导者提交多个日志条目时，跟随者可能不可用，然后它可以被选为领导者并用新的条目覆盖这些条目;结果，不同的状态机可能执行不同的命令序列。

在任何基于领导者的一致性算法中，领导者最终必须存储所有提交的日志条目。在一些共识算法中，例如Viewstamped Replition，即使领导者最初不包含所有提交的条目，也可以选出领导者。这些算法包含额外的机制来识别缺失的条目，并在选举过程中或之后不久将它们传送给新的领导者。不幸的是，这导致了相当大的额外机制和复杂性。 Raft使用一种更简单的方法，它保证从选举之时起，每个新领导者都会出现之前条款中的所有已提交条目，而无需将这些条目转移给领导者。这意味着日志条目只在一个方向上流动，从领导者到关注者，领导者永远不会覆盖日志中的现有条目。

Raft使用投票过程来阻止候选人赢得选举，除非其日志包含所有已提交的条目。候选人必须联系群集的大多数才能被选举，这意味着每个提交的条目必须至少存在于其中一个服务器中。如果候选人的日志至少与该多数中的任何其他日志一样是最新的（其中“最新”定义如下），则它将保留所有已提交的条目。 RequestVote RPC实现了这一限制：RPC包含有关候选人日志的信息，如果其自己的日志比候选人的日志更新，则选民拒绝其投票。

算法通常以正确性，效率和/或简洁性为主要目标而设计。虽然这些都是有价值的目标，但我们相信可理解性同样重要。在开发人员将算法渲染为实际实现之前，其他任何目标都无法实现，这将不可避免地偏离并扩展已发布的表单。除非开发人员对算法有深入的了解并且可以创建直觉，否则他们很难在实现中保留其理想的属性。

在本文中，我们讨论了分布式共识问题，其中一个被广泛接受但难以理解的算法Paxos多年来一直挑战学生和开发人员。我们开发了一种新的算法Raft，我们已经证明它比Paxos更容易理解。我们也相信Raft为系统构建提供了更好的基础。将可理解性作为主要设计目标改变了我们接近Raft设计的方式；随着设计的进步，我们发现自己重复使用了一些技术，例如分解问题和简化状态空间。这些技术不仅提高了Raft的可理解性，而且使我们更容易说服自己的正确性。


### 32. On Security Analysis of Proof-of-Elapsed-Time (PoET)

**关于经验证明（PoET）的安全性分析**

> 最近，英特尔提出了一种新的经过验证时间（PoET）概念，该概念利用可信计算来强制执行块构造的随机等待时间。但是，可信计算组件可能不完美且100％可靠。目前尚不清楚，基于PoET的区块链系统在多大程度上可以容忍可信计算组件的故障。 PoET的当前设计缺乏严格的安全性分析和评估其抵御此类攻击的力量的理论基础。为了实现这一差距，我们开发了一个评估基于PoET的区块链系统的理论框架，并表明当前的设计是脆弱的，因为攻击者可以通过仅损害Θ（log log n / log n）分数来危害区块链系统。参与节点，当n相对较大时非常小。根据我们的理论分析，我们还提出了缓解这些漏洞的方法。

可信计算技术提供了另一个改进区块链的表现的机会。可信计算利用特殊的硬件属性来提供可信的执行环境，其中攻击者无法篡改应用程序的执行。所有主要处理器供应商（如Intel，AMD和ARM）都有自己的可信计算解决方案。

基于其可信赖的计算平台SGX，英特尔提出了区块链构建的“经过时间证明”（PoET）的概念。基本思想是每个节点生成一个随机数，以确定在允许生成块之前必须等待多长时间。随机数的生成基于系统预先指定的某种分布。当新块提交给系统时，SGX帮助创建块的节点生成等待时间的证明。使用SGX技术的其他节点可以轻松验证此证明。统计测试用于确定等待时间是否确实遵循指定的分布。与PoW等其他区块链方案相比，这种方法有两大优势：（i）效率。在创建新块之前，PoET不要求参与节点执行昂贵的计算工作量; （ii）公平。 PoET实现了“一CPU一票”的目标，最初是在Nakamoto的比特币论文中提出的，但之前没有完全实现。

总之，我们在本文中的主要贡献包括：

- 我们开发了基于PoET的区块链系统的抽象模型，该模型捕获了PoET的关键特征，为PoET的理论分析和评估打开了大门;
- 我们分析了Sawtooth Lake Scheme的设计，发现即使在只有很小一部分节点受到损害的情况下，当前协议也很脆弱;
- 根据我们的分析，我们提供了基于PoET概念设计区块链方案的安全指南和建议。

值得指出的是，我们对PoET的分析侧重于理论和协议设计水平。该分析不依赖于任何特定的硬件实现缺陷或漏洞，因此通常具有这种缺陷。

英特尔的软件保护扩展（SGX）技术提供了一种机制，可以保护所选代码和数据免于泄露或修改。基于SGX，英特尔提出了Sawtooth Lake，它利用了“经过时间证明”的理念（PoET）控制新块的构造。使用此方案，每个用户必须等待一段时间才能允许创建块。这样的等待时间需要遵循由方案确定的概率分布F.简而言之，该方案使用两种措施来确保用户必须等待这样的时间。首先，每个用户一旦生成块，还需要在SGX硬件的帮助下生成等待活动的证明，SGX硬件与块一起提交。其次，采用统计测试来检查用户的等待时间是否确实遵循特定的概率分布。

随机等待时间如我们所描述的，在PoET方案中，每个节点必须在生成下一个块之前等待分布F之后的时间段。在目前由英特尔提出的Sawtooth Lake方法中，该F可以通过两阶段程序来表征。在较高级别，该过程如下工作。每个节点首先使用公式生成一个数字作为其临时等待时间。这样的等待时间可以用于生成多个块，直到它必须被更新。具体地说，每当节点使用临时等待时间生成块时，它随机决定是否也将使用该等待时间生成下一个块，即，以某个概率p，它重新生成新的等待时间，否则它继续使用当前的等待时间。

基于PoET的区块链系统的抽象模型。

- 该系统由n个节点（用户）组成，每个节点配备一个可信计算组件。每个节点都会生成块并将其添加到系统中。我们假设生成块所需的时间可以忽略不计。但是，一旦一个节点生成一个块，它必须等待一定的时间（称为等待时间）才能生成下一个节点。

**相关工作**：
> 根据2.1节中的讨论，主要的安全要求是容忍恶意用户。

作为最受欢迎的区块链构建方法，PoW已经接受了深入研究。在比特币的初始论文中，Nakamoto表明，当大多数用户诚实时，攻击者可以成功构建他/她自己的分支的概率随着分支位置的深度呈指数下降。Garay和Pass等人。进一步验证了这些安全功能。还开发了正式框架来研究基于PoW的区块链的性能与其安全级别之间的关系。然而，由于它与PoW的根本区别，这些结果不能应用于PoET。

还有一系列研究侧重于涉及采矿的用户的博弈论方面。从博弈论的角度来看，Eyal和Sirer表明，即使是大多数诚实的矿工也不足以保证比特币协议的安全性。 陈等人。进一步研究智能合约的执行作为一种游戏。所有这些工作都假设用户可以在PoW的限制下确定他们的行为，这不适用于PoET。对于PoET，攻击者要么被迫遵循协议（当可信计算硬件没有受到损害时），要么能够做任何他/她想做的事情（当可信计算硬件被泄露时）。
	

### 33. Proof of Luck: an Efficient Blockchain Consensus Protocol

**运气证明：一种有效的区块链共识协议**

> 在本文中，我们提出了多个区块链contimus原语和一个新颖的区块链系统的设计，所有这些都基于可信执行环境（TEE）的使用，例如支持英特尔SGX的CPU。 首先，我们展示了如何将TEE用于现有的工作方案证明，通过阻止使用ASIC，可以使采矿得到公平分配。 接下来，我们通过时间证明和所有权共识原语的证明来扩展设计，以使采矿能量和时间有效。 进一步改进这些设计，我们使用运气证明共识协议提出区块链。 我们的运气区块链证明使用TEE平台的随机数生成来选择共识领导者，它提供低延迟交易验证，确定性确认时间，可忽略的能源消耗以及公平分布式挖掘。 最后，我们讨论了针对一定数量的受损TEE的潜在保护。

为了解决这些缺点，我们可以使用现代可信执行环境（TEE）来建立新的共识原则，以用于分散的电子货币设计。 TEE的功能可以强制执行关键操作的正确处理，还可以限制在单个硬件单元下运行的Sybils的影响。

在本文中，我们提出了一种新颖的一致性算法，运气证明，以及使用它的概念验证区块链设计，它实现了低延迟的事务验证，同时在理性攻击者和最小的能量和计算能力下使用良性参与者。

我们的贡献如下：

- 我们提出了三个基本的共识原语，它们使用TEE证明工作，时间证明和所有权证明。这些是现有共识原语的节能直接替代品。
- 我们提出了一个新颖的第四个共识基本原理运气和区块链设计，使用它来实现低延迟交易验证，确定性确认时间，可忽略的能源消耗和可分配的采矿。
- 我们讨论了针对少数受到攻击的TEE的攻击者的潜在保护。

我们的目标是设计一个共识算法：

1.快速，确定的交易确认。<br>
2.能源和网络通信高效协议。<br>
3.耐受不常用的定制硬件。<br>
4.在TEE阈值下控制的攻击者无法控制区块链。<br>
5.攻击者无法在不控制大部分CPU且不破坏TEE平台的情况下控制区块链。<br>
6.参与者之间不需要同步时钟。<br>

结论：

我们已经为使用现有工作证明方案的系统提出了三种支持TEE的构建模块设计：支持TEE的工作证明，时间证明和所有权证明。 我们将这些原语的想法结合到基于运气共识协议的新区块链系统中。 我们的分析表明，我们的区块链可确保生存和持久性，同时提供节能挖掘，具有确定性确认时间的低延迟交易验证以及分散的挖掘能力。 最后，我们讨论了对参与区块链的一定数量的受损TEE的潜在保护。


### 34. Proof of Activity: Extending Bitcoin’s Proof of Work via Proof of Stake

**活动证明：通过股权证明扩展比特币的工作证明**

> 我们提出了一种新的加密货币协议，该协议建立在比特币协议的基础上，将其工作证明组件与证明类型的系统相结合。 我们的活动证明（PoA）协议为未来对比特币的可能实际攻击提供了良好的安全性，并且在网络通信和存储空间方面具有相对较低的惩罚。 我们探索各种攻击场景，并建议对PoA协议的潜在漏洞进行补救，并评估其核心子例程的性能。

强大的加密货币协议应该努力提供一种激励结构，在该激励结构下，系统中不同参与者的自身利益是维持其健康的。在这项工作中，我们提供了比特币协议的详细扩展，作为我们认为可能的安全威胁的补救措施，因为对扩展协议的攻击会更加昂贵。基本上，我们的分析和建议的补救措施源于PoW矿工没有正确的经济激励来完全负责保护网络的主张，并且利益相关者适合协助完成这项任务。我们提出的活动证明（PoA）协议也可能具有其他功能，例如促进增强的网络拓扑和更少的总体能耗。为了换取我们认为PoA协议实现的理想属性，PoA网络中的节点需要相对于比特币网络中的节点进行更多的工作和通信。

> PoA协议的目的是建立一个分散的cyrptocurrency网络，其安全性基于工作证明和股权证明的组合。

活动证明协议是比特币协议的扩展。与比特币网络节点的工作相比，PoA中的网络节点需要进行更复杂的验证，我们的论点是这些额外的工作带来了一些特殊的好处。

PoA所包含的主要子程序称为跟随式，我们将一些伪随机值转换为satoshi（加密货币的最小单位），该satoshi在迄今已铸造的所有satoshis中均匀选取。这是通过选择零到存在于最后一个块之前的satoshis总数之间的伪随机索引，检查创建该satoshi的块，并跟踪每个将该satoshi转移到后续地址的事务直到到达该地址来完成的。目前控制这个satoshi。

只有维持完整在线节点的活跃利益相关者才能获得奖励，以换取他们为网络提供的重要服务。

结论

PoA协议旨在分散以非常明显的方式同步事务的功率。 为了垄断块创建过程，攻击者需要控制到目前为止已经生成的硬币总量的很大一部分。 我们认为，在可能的情况下，PoA协议的攻击成本要高于比特币的纯PoW协议。 此外，PoA协议可能实现其他有益特性，即改进的网络拓扑，维持完整在线节点的激励，低交易费用和更有效的能量使用。

