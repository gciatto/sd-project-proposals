Proposed Projects for the Distributed Systems course
====================================================

[Giovanni Ciatto](mailto:giovanni.ciatto@unibo.it), 
[Stefano Mariani](mailto:s.mariani@unibo.it), 
[Andrea Omicini](mailto:andrea.omicini@unibo.it)

Overview
--------

Proposed projects are divided into the following main categories:

**Tuple Based coordination**, where students may contribute in several
ways to our software artifacts concerning the tuple based coordination,
i.e.:

[**TuSoW**](http://apice.unibo.it/xwiki/bin/download/Publications/TusowIcccn2019/08846916.pdf):
the same LINDA implementation you used during the Lab lessons

-   Source code avaiable here: <https://github.com/tuple-based-coord/TuSoW/>
    * heavily based on Kotlin

[**TuCSoN**](http://apice.unibo.it/xwiki/bin/view/TuCSoN/WebHome):
another legacy implementation of LINDA, which is and has been the basis
for several research works in our team. In particular, it supports not
only tuple spaces but also [tuple
centres](http://apice.unibo.it/xwiki/bin/view/Publications/RespectScp41)

-   You can read more about TuCSoN and the tuple centre notion by
    looking for the many papers mentioning them among the [ones
    published by prof.
    Omicini](http://apice.unibo.it/xwiki/bin/view/AndreaOmicini/Publications)

    -   **log in** with your `@studio.unibo.it` credentials on the
        **Apice** portal, in order to be able to download and read our
        papers
-   Or you may look for the many theses on these subjects available on
    [AMS Tesi](https://amslaurea.unibo.it/cgi/search/simple?q=tucson&_action_search=Search&_order=bytitle&basic_srchtype=ALL&_satisfyall=ALL)

[**ReSpecT**](http://apice.unibo.it/xwiki/bin/view/ReSpecT/WebHome): a
language aimed at programming tuple centres in order to govern the
*interaction space*

-   A good starting point for developers:
    <http://apice.unibo.it/xwiki/bin/view/Publications/RespectxComsis15>
-   Formal semantics:
    <http://apice.unibo.it/xwiki/bin/view/Publications/RespectEntcs175>
-   Again, have a look to the many theses about it on AMS Tesi

**Logic Programming as a Service *(LPaaS)***, where students may
contribute in several ways to our software artifacts concerning the
LPaaS ecosystem

-   Put it simply, LPaaS leverages a Logic Programming engine (e.g.
    [`tuProlog`](http://tuprolog.unibo.it/)) wrapped by a ReSTful web service
-   Some interesting details are provided here:
    <http://apice.unibo.it/xwiki/bin/view/Publications/LpaasBdcc2>

**Blockchain**, where students may contribute in several ways in order
to improve their (and our) understanding of the **Blockchain** model and
technology

**[Byzantine] Fault Tolerance *([B]FT)* & State Machine Replication
*(SMR)***, where students may contribute in several ways in order to
improve our understanding of the BFT & SMR models and technologies

**Language and frameworks for Distributed Systems *(DS)* or Agent
Oriented Programming *(AOP)***, where students may contribute in several
ways in order to create or improve new languages or toolkits within the
scopes of DS, Coordination, and AOP

-   Projects in this category may rely on one or more of the following
    frameworks:

    -   [ANTLR](https://www.antlr.org/)
    -   [Xtext](https://www.eclipse.org/Xtext/)
    -   JetBrains' [MPS](https://www.jetbrains.com/mps/)
    -   Swagger's [Codegen](https://swagger.io/tools/swagger-codegen/)

**Simulation**: where students may contribute by
creating novel *incarnations* for the [**Alchemist**
simulator](http://alchemistsimulator.github.io/)

**DevOps**: where students can practice with real-world DevOps technologies such as Docker and Kubernetes

**Lesson Production**: where students can help designing and writing lessons for the future editions of the course

**Technology Know-How**: where students may contribute exploring the
functioning (and possibly the internal structure) of one or more
real-world technologies

The "Tuple Based coordination" category
---------------------------------------

This category comprehends the following projects

1.  Designing and implementing a
    [RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)
    access control feature for TuSoW, to be enforced by means of an
    authentication and authorization layer to be injected into the
    current model and implementation

    -   The implementation should rely on standard technologies such as
        [SSO](https://en.wikipedia.org/wiki/Single_sign-on) or
        [OAuth](https://it.wikipedia.org/wiki/OAuth)

2.  Designing and implementing a variant of TuSoW supporting the
    [**replication**](https://en.wikipedia.org/wiki/State_machine_replication)
    of tuple spaces on several distributed machines

    -   This may also mean creating/looking for a Storage Layer for
        TuSoW to be injected into the current model & implementation

3.  Designing and implementing a variant of TuSoW supporting the
    [**sharding**](https://en.wikipedia.org/wiki/Shard_%28database_architecture%29)
    of tuple spaces on several distributed machines

    -   This may also mean creating/looking for a Storage Layer for
        TuSoW to be injected into the current model & implementation

<!-- 4.  Designing and implementing a server-side interface for LINDA (or
    TuSoW core) to be wrapped within some IoT ready interface base on:

    1.  [gRPC](https://grpc.io/),
    2.  or [MQTT](https://en.wikipedia.org/wiki/MQTT),
    3.  or
        [AMQP](https://en.wikipedia.org/wiki/Advanced_Message_Queuing_Protocol)

    (notice that these are actually three different projects) -->
4.  Designing and implementing a server-side interface for LINDA (or
    TuSoW core) based on Javalin
        + simple project, max 1 person

5.  Designing and implementing a client-side interface for TuSoW
    supporting two or more of the follwing platforms:

    1.  JVM (Java, Kotlin, Scala, etc)
    2.  .NET (C\#, F\#, VbNET \<-- please don't)
    3.  JavaScript
    4.  Python
    5.  \< any language you like \>

    (notice that these are actually different projects)

    > Teams composed by more than 1 people may be asked to support more than 1 plaftorms 

6.  Designing and implementing an **observability** module for TuSoW
    enabling the implementation of a Web-based **monitoring**
    (graphical) interface, targetting:
        - JavaFX
        - some web GUI
    
    (notice that this activity may require some modification to the current implementation of TuSoW service)

7.  Designing and implementing an **Android**-based *porting* of TuSoW
    supporting [**replication**](https://en.wikipedia.org/wiki/State_machine_replication)
    of tuple spaces among several devices, possibly interconnected by
    means of Bluetooth or Wifi-Direct
        - there are some ongoing activities on this track, yet if you are interested let's talk about it

8.  Designing and implementing an **Android**-based *porting* of TuSoW
    supporting **federation** of tuple spaces *à la
    [LIME](https://dl.acm.org/citation.cfm?id=302659)* among several
    devices, possibly interconnected by means of Bluetooth or
    Wifi-Direct
        - there are some ongoing activities on this track, yet if you are interested let's talk about it

10. Fix the "phantom in" problem by supporting primitives cancellation from the client side in TuSoW
    - https://gitlab.com/pika-lab/tuples/coordination/-/issues/14

11. Experiment with novel Coordination languages in TuSoW, e.g.
    - JSON|YAML and JsonPAth
    - XML and XPath
    - whatever you like

The "LPaaS" category
--------------------

1.  Completely rewriting the current [Java EE based source
    code](https://gitlab.com/pika-lab/lpaas/lpaas-ws) using Javalin, Vert.x or
    some other lightweight, micro-service oriented library or framework.
    The novel implementation should include at least:

    -   an improved modularization of the Knowledge-Base Layer
    -   a suite of fine grained unit tests

    Notice that the novel implementation should anyway adhere to the
    [`LPaaS Swagger Specification`](https://app.swaggerhub.com/apis/PIKA-lab/LPaaS/1)

2.  Designing and implementing an **observability** module for LPaaS
    enabling the implementation of a Web-based graphical interface

3.  Designing and implementing a client-side interface for LPaaS
    supporting one of the follwing platforms:
    1. JVM
    1.  .NET (C\#, F\#, VbNET \<-- please don't)
    2.  Python

    (notice that these are actually different projects)


4. Design a novel [2P-Kt Playground](https://pika-lab.gitlab.io/tuprolog/2p-kt-web/) capable of switching among in-browser or LPaaS-based computing mode

Furthermore, we are also interested in students designing and developing
an **unbiased** and *non-trivial* usage scenario for LPaaS. You can
propose some.

The "Blockchain" category
-------------------------

No specific project here, but just some ideas you can use as a starting
point when proposing a project of yours.

We have four different rearch interestes concerning blockchains:

-   Extending the common notion of smart contract, in order to support
    asynchrony and time-reactiveness as a first step towards
    *autonomous* smart contracts

    -   More info here: <http://apice.unibo.it/xwiki/bin/view/Theses/BlockchainMaffi2018>

-   Experimenting and reproducing Hyperledger Fabric's **Execute-Order-Validate** architecture over [Tenderfone](http://apice.unibo.it/xwiki/bin/view/Theses/BlockchainMaffi2018)

    -   More info here: <https://arxiv.org/pdf/1801.10228.pdf>

-   Port [Tenderfone](http://apice.unibo.it/xwiki/bin/view/Theses/BlockchainMaffi2018) over [2P-Kt](https://github.com/tuProlog/2p-kt)
    - Tenderfone source code: <https://gitlab.com/pika-lab/blockchain/tenderfone/tenderfone-sc>

-   Formalising the [Ethereum Blockchain
    Platform](https://www.ethereum.org/) by means of the
    [ABS](https://link.springer.com/chapter/10.1007/978-3-642-25271-6_8)
    formalism

-   Creating (i.e. designing & implementing) our home-made
    **logic-based** blockchain technology from scratch, possibly relying
    on some Fault Tolerant layer such as:

    -   [BFT-Smart](http://bft-smart.github.io/library)
    -   Some [RAFT implementation](https://raft.github.io/#implementations)
    -   [Tendermint](https://tendermint.com/)

The "BFT & SMR" category
------------------------

Projects in this category follow a common pattern:

1.  Students choose a **consensus** algorithm from the list below,
2.  They study the corresponding paper / reference and try to understand
    the consensus algorithm's functioning
3.  They create a proof of concept implementation it using a technology
    of choice
4.  They test the consensus algorithm's robustness agains crash and
    byzantine faults

There is an implic step hidden into the procedure above: consensus
algorithms are usually aimed at implementing some sort of SMR system
(e.g. a replicated DB). Even if the goal of a project in this category
is to study & implement a consensus algorithm, students may need to
actually use it in order to test it. To do so they will have to create a
simple SMR system, like, e.g. a replicated Key-Value store supporting at
least two operations: `put` and `get`.

Students may choose any of the following consensus algorithms:

-   **PBFT**, [Castro, M., & Liskov, B. (2002). Practical byzantine
    fault tolerance and proactive
    recovery](https://www.microsoft.com/en-us/research/wp-content/uploads/2017/01/p398-castro-bft-tocs.pdf)
-   ~~**Honey Badger**, [Miller, A., Xia, Y., Croman, K., Shi, E., & Song,
    D. (2016). The Honey Badger of BFT
    Protocols](https://eprint.iacr.org/2016/199.pdf)~~
-   **BFT2F**, [Li, J., & Mazières, D. (2007). Beyond one-third faulty
    replicas in Byzantine fault tolerant
    systems](http://www.scs.stanford.edu/~jinyuan/bft2f.pdf)
-   ~~**Zyzzyva**, [Kotla, R., Alvisi, L., Dahlin, M., Clement, A., &
    Wong, E. (2007). Zyzzyva: Speculative Byzantine Fault
    Tolerance](http://sosp2007.org/papers/sosp052-kotla.pdf)~~
-   **Q/U**, [Abd-El-Malek, M., Ganger, G. R., Goodson, G. R., Reiter,
    M. K., & Wylie, J. J. (2005). Fault-scalable Byzantine
    fault-tolerant
    services](https://cs.brown.edu/courses/csci2950-g/papers/qu.pdf)
-   **Sieve**, [Cachin, C., Schubert, S., & Vukolić, M. (2016).
    Non-determinism in Byzantine Fault-Tolerant
    Replication](https://allquantor.at/blockchainbib/pdf/cachin2016non.pdf)
-   **Mastercrypt**, [Cachin, C., Schubert, S., & Vukolić, M. (2016).
    Non-determinism in Byzantine Fault-Tolerant
    Replication](https://allquantor.at/blockchainbib/pdf/cachin2016non.pdf)
    (yes, the same paper of Sieve)
-   **Mod Smart**, [Sousa, J., & Bessani, A. (2012). From Byzantine
    consensus to BFT state machine replication: A latency-optimal
    transformation](http://www.di.fc.ul.pt/~bessani/publications/edcc12-modsmart.pdf)
-   **HQ**, [Bershad, B., ACM Digital Library., D., ACM Special Interest
    Group in Operating Systems., B., Rodrigues, R., & Shrira, L. (2006).
    HQ Replication: A Hybrid Quorum Protocol for Byzantine Fault
    Tolerance](https://people.csail.mit.edu/cowling/hq/hq-osdi06.pdf)
-   ~~**RAFT**, [Diego Ongaro and John Ousterhout, (2014). In Search of an
    Understandable Consensus Algorithm](https://raft.github.io/raft.pdf)~~
-   **BFT-Smart** <https://github.com/bft-smart/library>
-   Google's **Chubby** <https://static.googleusercontent.com/media/research.google.com/it//archive/chubby-osdi06.pdf>

Overviews and surveys are available in order to perform a quick
evaluation and comparison among the protocols above:

-   [Cachin, C., & Vukolić, M. (2017). "Blockchain Consensus Protocols
    in the Wild"](https://arxiv.org/pdf/1707.01873.pdf)
-   [Aublin, P.-L., Guerraoui, R., Knežević, N., Quéma, V., & Vukolić,
    M. (2015). The Next 700 BFT Protocols. ACM Transactions on Computer
    Systems, 32(4),
    1–45](https://infoscience.epfl.ch/record/121590/files/TR-700-2009.pdf)
-   [Sankar, L. S., Sindhu, M., & Sethumadhavan, M. (2017). Survey of
    consensus protocols on blockchain
    applications](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8014672)
-   [Malkhi, D., & Reiter, M. (1998). Byzantine quorum
    systems](https://www.cs.unc.edu/~reiter/papers/1998/DC.pdf)

Finally, the following readings may of interest for who is interest in
understanding the many impossiblity results affecting the distributed
consensus:

-   [Fischer, M. J.; Lynch, N. A.; Paterson, M. S. (1985).
    "Impossibility of distributed consensus with one faulty
    process"](https://www.the-paper-trail.org/post/2008-08-13-a-brief-tour-of-flp-impossibility/)
-   [Lamport, L.; Shostak, R.; Pease, M. (1982). "The Byzantine Generals
    Problem"](https://people.eecs.berkeley.edu/~luca/cs174/byzantine.pdf)
-   Chapters 7, 8, 9 of Tanenbaum & van Steen's "Distributed Systems"
    book

The "Language & frameworks for DS or AOP" category
--------------------------------------------------

1.  Design and implement a plugin for Swagger's Codegen aimed at
    generating server stubs starting from a Swagger specification file.
    
        - Vert.X target
        - Javalin target
        - Play target
        - choose your own target

2.  Design and implement a Domain Specific Language aimed at easing the
    development of JADE-like agents

    -   It is possible to use any one among the following DSL
        engineering technologies: Xtext, MPS, ANTLR

4. Design a Kotlin|Scala DSL for Jade-like Agents


The "Simulation" category
-------------------------

1.  Design and implement an Alchemist incarnation aimed at simulating
    situated tuple spaces and, possibly, the [Spatial Tuples
    model](https://link.springer.com/chapter/10.1007/978-3-319-48829-5_12)

2.  Design and implement an Alchemist incarnation aimed at simulating
    situated tuple **centres**

3.  Design and implement an Alchemist incarnation aimed at simulating
    JADE-like agents

DevOps category
---------------

Projects in this category follow a common pattern:

1.  Students choose a **technology** from the list below aimed at setting up clusters of interconnected machines,

0.  They must study it and understand its purpose & functioning,
    possibly looking for scientific paper describing it

0.  They must figure out and document how to set up a single-machine cluster

0.  They must figure out and document how to set up a multi-machine cluster

0.  They must figure out and document how to set up access control and usage quotas

0.  They must figure out and document how to submit computational jobs to the cluster

0.  They must figure out and document how to submit storage-intensive jobs to the cluster

0.  They must figure out and document how to deploy web-services or super-servers on the cluster

Avalilable technologies:

- [Docker Swarm](https://docs.docker.com/engine/swarm/)
- [Kubernetes](https://kubernetes.io)

Lesson Production category
--------------------------

1. Design a lab lesson about __replication__ of Linda tuple spaces
    - master-slave
    - crash-tolerant
    - BFT

0. Design a lab lesson about __federation__ of Linda tuple spaces

0. Design a lab lesson about __sharding__ of Linda tuple spaces

0. Design a lab lesson non-blocking IO

0. Propose your own lab lesson to be designed

The "Technology Know-How" category
----------------------------------

Projects in this category follow a common pattern:

1.  Students choose a **technology** from the list below,

2.  They must study it and understand its purpose & functioning,
    possibly looking for scientific paper describing it

3.  They must undestand how the technology setup works and it is
    deployed in a real-world scenario

    -   [Docker Swarm](https://docs.docker.com/engine/swarm/) may be
        useful in some cases
    -   Such information must be included into the final report

4.  They must test it, possibly creating some non-trivial testbed
    scenario

    -   It is not sufficient to just copy & past examples from the Web
    -   The test bed scenario must be propertly designed in order to
        reveal the technology pros and cons

5.  They must stress it, possibly creating some testbed pushing the
    technology out of its comfort zone

6.  They must produce a detailed report describing

    -   the technology,
    -   its reference model (if any),
    -   the assumption it relies upon,
    -   the tests performed and their rationale,
    -   the problems it solves
    -   the problems it DOES NOT solve
    -   etc

Avalilable technologies:

-   ~~[Docker Swarm](https://docs.docker.com/engine/swarm/)~~
-   [Traefik](https://traefik.io/)
-   [Etcd](https://coreos.com/etcd/)
-   ~~[CEPH](https://ceph.com/)~~
-   ~~[Redis](https://redis.io/)~~
-   ~~[Lagom](https://www.lagomframework.com/) and, in particular, its
    [Event Sourcing](https://www.lagomframework.com/documentation/1.4.x/java/ESAdvantage.html) feature~~
-   [Apache Flink](https://flink.apache.org/)
-   ~~[Apache Kafka](https://kafka.apache.org/)~~
-   [Apache ZooKeeper](https://zookeeper.apache.org/)
-   [IPFS -- Inteplanetary File System](https://ipfs.io/)
-   [Storj](https://storj.io/)

Notice that projects in this category are quite different. Here, we only
expect students to produce some non-trivial testbed + some other code
examples as software artifacts. The real goal of this sort of projects
is to condensate into some useful and written form the knowledge related
to a particular technology. Because of this, the final repor **must** be
very detailed and properly written, **without assuming the reader have
any prior knowledge concerning the technology presented into the
report**. For this reason **final report have no page limitation in this
category**.

Notice that **technicalities are *not* the only thing that matters**.
This is why we ask you to reason about a technology, and think about:

-   why should people use it?
-   why people should NOT use it?
-   does it scale?
-   etc.

As a rule of thumb consider the following statement:

> *if your report does not present any problem of the target technology,
> you are probably missing something*


