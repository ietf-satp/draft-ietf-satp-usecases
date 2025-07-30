---

stand_alone: yes
pi:
  rfcedstyle: yes
  toc: yes
  tocindent: yes
  tocdepth: 4
  sortrefs: yes
  symrefs: yes
  strict: yes
  comments: yes
  inline: yes
  text-list-symbols: o-*+
  compact: yes
  subcompact: no

title: Secure Asset Transfer (SAT) Use Cases
abbrev: SAT Use Cases
docname: draft-ietf-satp-usecases-latest
category: info

ipr: trust200902
area: "Applications and Real-Time"
workgroup: "Secure Asset Transfer Protocol"

stream: IETF
keyword: Internet-Draft
consensus: true

venue:
  group: "Secure Asset Transfer Protocol"
  type: "Working Group"
  mail: "sat@ietf.org"
  arch: "https://mailarchive.ietf.org/arch/browse/sat/"
  github: "ietf-satp/draft-ietf-satp-usecases"
  latest: "https://ietf-satp.github.io/draft-ietf-satp-usecases/draft-ietf-satp-usecases.html"

author:
  -
    ins: V. Ramakrishna
    name: Venkatraman Ramakrishna
    organization: IBM Research
    email: vramakr2@in.ibm.com
  -
    ins: T. Hardjono
    name: Thomas Hardjono
    organization: MIT
    email: hardjono@mit.edu
  -
    ins: C. Liu
    name: Chunchi (Peter) Liu
    organization: Huawei
    email: liuchunchi@huawei.com

informative:
  Abebe19:
    author:
    - ins: E. Abebe
    - ins: D. Behl
    - ins: C. Govindarajan
    - ins: Y. Hu
    - ins: D. Karunamoorthy
    - ins: P. Novotny
    - ins: V. Pandit
    - ins: V. Ramakrishna
    - ins: C. Vecchiola
    date: December 2019
    target: https://arxiv.org/abs/1911.01064
    title: Enabling Enterprise Blockchain Interoperability with Trusted Data Transfer (Middleware 2019 - Industry Track)
  Abebe21:
    author:
    - ins: E. Abebe
    - ins: Y. Hu
    - ins: A. Irvin
    - ins: D. Karunamoorthy
    - ins: V. Pandit
    - ins: V. Ramakrishna
    - ins: J. Yu
    date: May 2021
    target: https://arxiv.org/abs/2012.07339
    title: Verifiable Observation of Permissioned Ledgers (ICBC 2021)
  ABCH20:
    author:
    - ins: T. Ankenbrand
    - ins: D. Bieri
    - ins: R. Cortivo
    - ins: J. Hoehener
    - ins: T. Hardjono
    date: May 2020
    target: https://arxiv.org/abs/2007.11877
    title: Proposal for a Comprehensive Crypto Asset Taxonomy
  BSN22:
    author:
    - ins: A. Kharpal
    date: May 2022
    target: https://www.cnbc.com/2022/05/16/china-blockchain-explainer-what-is-bsn-.html
    title: China has been quietly building a blockchain platform. Here’s what we know. CNBC
  BVGC20:
    author:
    - ins: R. Belchior
    - ins: A. Vasconcelos
    - ins: S. Guerreiro
    - ins: M. Correia
    date: May 2020
    target: https://arxiv.org/abs/2005.14282v2
    title: 'A Survey on Blockchain Interoperability: Past, Present, and Future Trends'
  CDE23:
    author:
    - ins: S. Bhardwaj
    date: August 2023
    target: https://www.forbesindia.com/article/cryptocurrency/china-unveils-revolutionary-blockchain-data-exchange-at-hangzhou-summit/87745/1
    title: China Unveils Revolutionary Blockchain Data Exchange at Hangzhou Summit. Forbes India
  Clar88:
    author:
    - ins: D. Clark
    date: August 1988
    title: The Design Philosophy of the DARPA Internet Protocols, ACM Computer Communication Review, Proc SIGCOMM 88, vol. 18, no. 4, pp. 106-114
  Gray81:
    author:
    - ins: J. Gray
    date: September 1981
    title: 'The Transaction Concept: Virtues and Limitations, in VLDB Proceedings of the 7th International Conference, Cannes, France, September 1981, pp. 144-154'
  Herl19:
    author:
    - ins: M. Herlihy
    date: February 2019
    target: https://doi.org/10.1145/3209623
    title: Blockchains from a Distributed Computing Perspective, Communications of the ACM, vol. 62, no. 2, pp. 78-85
  HLP19:
    author:
    - ins: T. Hardjono
    - ins: A. Lipton
    - ins: A. Pentland
    date: June 2019
    target: https://doi:10.1109/TEM.2019.2920154
    title: Towards and Interoperability Architecture for Blockchain Autonomous Systems, IEEE Transactions on Engineering Management
  HS2019:
    author:
    - ins: T. Hardjono
    - ins: N. Smith
    date: December 2019
    target: https://doi.org/10.3389/fbloc.2019.00024
    title: Decentralized Trusted Computing Base for Blockchain Infrastructure Security, Frontiers Journal, Special Issue on Blockchain Technology, Vol. 2, No. 24
  HTLC21:
    author:
    date:
    target: https://en.bitcoin.it/wiki/Hash_Time_Locked_Contracts
    title: Hash Time Locked Contracts, Bitcoin Wiki
  IDevID:
    author:
    - ins: M. Richardson
    - ins: J. Yang
    date: August 2020
    target: https://tools.ietf.org/html/draft-richardson-t2trg-idevid-considerations-01
    title: A Taxonomy of operational security of manufacturer installed keys and anchors. IETF draft-richardson-t2trg-idevid-considerations-01
  SRC84:
    author:
    - ins: J. Saltzer
    - ins: D. Reed
    - ins: D. Clark
    date: November 1984
    title: End-to-End Arguments in System Design, ACM Transactions on Computer Systems, vol. 2, no. 4, pp. 277-288

normative:
  Aug23:
    author:
    - ins: A. Augusto
    - ins: R. Belchior
    - ins: I. Kocsis
    - ins: L. Gönczy
    - ins: A. Vasconcelos
    - ins: M. Correia
    date: 2023
    target: https://www.techrxiv.org/articles/preprint/CBDC_bridging_between_Hyperledger_Fabric_and_permissioned_EVM-based_blockchains/21809430
    title: '2023 IEEE International Conference on Blockchain and Cryptocurrency (ICBC), Dubai, United Arab Emirates, 2023, pp. 1-9 (doi: 10.1109/ICBC56567.2023.10174953)'
  BISCBDC:
    author:
    - ins: Bank of Canada
    - ins: European Central Bank
    - ins: Bank of Japan
    - ins: Sveriges Riksbank
    - ins: Swiss National Bank
    - ins: Bank of England
    - ins: Board of Governors of the Federal Reserve
    - ins: Bank for International Settlements
    date: October 2020
    target: https://www.bis.org/publ/othp33.htm
    title: 'Central bank digital currencies: foundational principles and core features. Bank for International Settlements, BIS Report'
  BISCBP:
    author:
    - ins: Bank for International Settlements
    - ins: Committee on Payments and Market Infrastructures
    - ins: Innovation Hub
    - ins: International Monetary Fund
    - ins: World Bank Group
    date: July 2021
    target: https://www.bis.org/publ/othp38.htm
    title: Central bank digital currencies for cross-border payments. Bank for International Settlements, Report to the G20
  BISDeFi:
    author:
    - ins: R. Auer
    - ins: B. Haslhofer
    - ins: S. Kitzler
    - ins: P. Saggese
    - ins: F. Victor
    target: https://www.bis.org/publ/work1066.htm
    title: The Technology of Decentralized Finance (DeFi). Bank for International Settlements, BIS Working Paper No. 1066
  BISMCBDC:
    author:
    - ins: R. Auer
    - ins: P. Haene
    - ins: H. Holden
    date: March 2021
    target: https://www.bis.org/publ/bppdf/bispap115.htm
    title: Multi-CBDC arrangements and the future of cross-border payments. Bank for International Settlements, BIS Paper No. 115
  BISRCBDC:
    author:
    - ins: R. Auer
    - ins: R. Boehme
    date: March 2020
    target: https://www.bis.org/publ/qtrpdf/r_qt2003j.htm
    title: The technology of retail central bank digital currency. Bank for International Settlements, BIS Quarterly Review
  BKYC:
    author:
    - ins: K. Bhaskaran
    - ins: P. Ilfrich
    - ins: D. Liffman
    - ins: C. Vecchiola
    - ins: P. Jayachandran
    - ins: A. Kumar
    - ins: F. Lim
    - ins: K. Nandakumar
    - ins: Z. Qin
    - ins: V. Ramakrishna
    - ins: E. GS Teo
    - ins: C. H. Suen
    date: April 17, 2018
    title: Double-Blind Consent-Driven Data Sharing on Blockchain. First IEEE Workshop on Blockchain Technologies and Applications (BTA) 2018, Co-located with 2018 IEEE International Conference on Cloud Engineering (IC2E)
  CatenaX:
    author:
    - ins: Catena-X
    date: 2025
    target: https://catena-x.net/
    title: Catena-X is the first globally trusted and collaborative data ecosystem for the automotive industry
  CNDatInf:
    author:
    - ins: Xinhua
    date: November 2024
    target: https://english.www.gov.cn/news/202411/23/content_WS67417342c6d0868f4e8ed59e.html
    title: Data infrastructure blueprint unveiled
  CNMeas:
    author:
    - ins: Xinhua
    date: December 2022
    target: https://english.www.gov.cn/policies/latestreleases/202212/19/content_WS63a17f7dc6d0a757729e49bd.html
    title: China unveils measures to build basic systems for data
  DSP:
    author:
    - ins: International Data Spaces Association
    date: 2025
    target: https://internationaldataspaces.org/offers/dataspace-protocol/
    title: 'Advancing interoperability: the Dataspace Protocol'
  EclDS:
    author:
    - ins: Eclipse Foundation
    date: 2025
    target: https://projects.eclipse.org/working-group/eclipse-dataspace
    title: Eclipse Dataspace Working Group
  ERC721:
    author:
    - ins: Ethereum.org
    date: November 19, 2023
    target: https://ethereum.org/en/developers/docs/standards/tokens/erc-721/
    title: ERC-721 Non-Fungible Token Standard.
  Ethereum:
    author:
    target: https://ethereum.org/
    title: Ethereum
  GaiaX:
    author:
    - ins: Gaia-X, European Association for Data and Cloud AISBL
    date: 2025
    target: https://gaia-x.eu/wp-content/uploads/2025/01/Gaia-X-Brochure_Overview-2025.pdf
    title: Together towards a federated and secure data infrastructure
  GoDaddy:
    author:
    - ins: GoDaddy
    date: 2024
    target: https://www.godaddy.com/
    title: Domain Names, Websites, Hosting & Online Marketing Tools.
  HLB:
    author:
    target: https://www.lfdecentralizedtrust.org/projects/besu
    title: Hyperledger Besu
  HLC:
    author:
    - ins: P. Somogyvari
    - ins: J. S. Sasan
    - ins: I. Sato
    - ins: T. Takeuchi
    - ins: V. Ramakrishna
    - ins: S. Nishad
    - ins: K. Narayanam
    - ins: D. Vinayagamurthy
    date: November 2022
    target: https://www.lfdecentralizedtrust.org/blog/2022/11/07/introducing-hyperledger-cacti-a-multi-faceted-pluggable-interoperability-framework
    title: Introducing Hyperledger Cacti, a multi-faceted pluggable interoperability framework. Linux Foundation Decentralized Trust Blog
  HLF:
    author:
    - ins: E. Androulaki
    - ins: A. Barger
    - ins: V. Bortnikov
    - ins: C. Cachin
    - ins: K. Christidis
    - ins: A. De Caro
    - ins: D. Enyeart
    - ins: C. Ferris
    - ins: G. Laventman
    - ins: Y. Manevich
    - ins: S. Muralidharan
    - ins: C. Murthy
    - ins: B. Nguyen
    - ins: M. Sethi
    - ins: G. Singh
    - ins: K. Smith
    - ins: A. Sorniotti
    - ins: C. Stathakopoulou
    - ins: M. Vukolic
    - ins: S. Weed Cocco
    - ins: J. Yellick
    date: April 2018
    target: https://dl.acm.org/doi/pdf/10.1145/3190508.3190538
    title: 'Hyperledger Fabric: A Distributed Operating System for Permissioned Blockchains (EuroSys 2018)'
  IDSA:
    author:
    - ins: International Data Spaces Association
    date: 2025
    target: https://internationaldataspaces.org/why/international-standards/
    title: 'International Standards: Worldwide access, European principles'
  IFT:
    author:
    - ins: IBM
    date: 2022
    target: https://www.ibm.com/docs/en/food-trust
    title: IBM Food Trust – Blockchain for the world’s food supply
  ISO:
    author:
    - ins: ISO
    date: July 2020
    target: https://www.iso.org/standard/82208.html
    title: Blockchain and distributed ledger technologies-Vocabulary (ISO:22739:2020)
  MP:
    author:
    - ins: P. Ignatova
    date: 2022
    target: https://www.tradefinanceglobal.com/posts/marco-polo-network-successfully-completes-largest-blockchain-open-account-trade-finance-trial-on-r3s-corda-platform/
    title: Marco Polo Network successfully completes largest Blockchain Open Account Trade Finance Trial on R3’s Corda platform, Trade Finance Global
  NIST:
    author:
    - ins: D. Yaga
    - ins: P. Mell
    - ins: N. Roby
    - ins: K. Scarfone
    date: October 2018
    target: https://doi.org/10.6028/NIST.IR.8202
    title: NIST Blockchain Technology Overview (NISTR-8202)
  OCC:
    author:
    - ins: Adam Hayes
    date: October 6, 2022
    target: https://www.investopedia.com/terms/o/occ.asp
    title: 'Options Clearing Corporation (OCC): Meaning, Overview, History (Investopedia)'
  PUbin:
    author:
    - ins: Bank of America Merrill Lynch
    - ins: BCS Information Systems
    - ins: Credit Suisse
    - ins: DBS Bank
    - ins: HSBC
    - ins: J.P. Morgan
    - ins: Mitsubishi UFJ Financial Group
    - ins: OCBC Bank
    - ins: R3
    - ins: Singapore Exchange
    - ins: UOB Bank
    date: 2017
    target: https://www2.deloitte.com/content/dam/Deloitte/sg/Documents/financial-services/sg-fsi-project-ubin-report.pdf
    title: 'The future is here: Project Ubin: SGD on Distributed Ledger. Deloitte and Monetary Authority of Singapore (MAS), Report'
  R3C:
    author:
    - ins: M. Hearn
    - ins: R. G. Brown
    date: August 2019
    target: https://docs.r3.com/en/pdf/corda-technical-whitepaper.pdf
    title: 'Corda: A Distributed Ledger'
  RFC1034: RFC1034
  RFC1035: RFC1035
  RFC5730: RFC5730
  SATA:
    author:
    - ins: T. Hardjono
    - ins: M. Hargreaves
    - ins: N. Smith
    - ins: V. Ramakrishna
    date: June 2025
    target: https://datatracker.ietf.org/doc/draft-ietf-satp-architecture/
    title: Secure Asset Transfer (SAT) Interoperability Architecture, IETF, draft-ietf-satp-architecture-07
  SATP:
    author:
    - ins: M. Hargreaves
    - ins: T. Hardjono
    - ins: R. Belchior
    - ins: V. Ramakrishna
    date: July 2025
    target: https://datatracker.ietf.org/doc/draft-ietf-satp-core/
    title: Secure Asset Transfer Protocol (SATP) Core, IETF, draft-ietf-satp-core-10
  SKYC:
    author:
    - ins: M. Curry
    date: August 7, 2018
    target: https://www.linkedin.com/pulse/blockchain-kyc-game-changing-regtech-innovation-michael-curry/
    title: 'Blockchain for KYC: Game-changing RegTech innovation'
  SSpace:
    author:
    - ins: Squarespace Domains
    date: 2024
    target: https://domains.squarespace.com/
    title: Domain Name Search – Register Your Domain Name.
  STN:
    author:
    - ins: Stellar Development Foundation
    date: 2022
    target: https://www.stellar.org/
    title: Stellar – Access your universe of opportunities
  StOpt:
    author:
    - ins: Investopedia
    date: 2024
    target: https://www.investopedia.com/terms/s/stockoption.asp
    title: What Are Stock Options? Parameters and Trading, With Examples
  TL:
    author:
    - ins: TradeLens
    date: 2022
    target: https://www.tradelens.com/
    title: 'TradeLens: Supply chain data and docs'
  VSign:
    author:
    - ins: Verisign
    date: 2024
    target: https://www.verisign.com/
    title: Verisign is a global provider of domain name registry services and internet infrastructure.
  WBGCBP:
    author:
    date: November 2021
    target: https://documents1.worldbank.org/curated/en/369001638871862939/pdf/Central-Bank-Digital-Currencies-for-Cross-border-Payments-A-Review-of-Current-Experiments-and-Ideas.pdf
    title: 'Central Bank Digital Currencies for Cross-Border Payments: A Review of Current Experiments and Ideas. World Bank Group, Other Financial Sector Study'
  Web3:
    author:
    - ins: Wikipedia
    date: 2024
    target: https://en.wikipedia.org/wiki/Web3
    title: Web3
  WET:
    author:
    - ins: IBM
    date: 2019
    target: https://www.ibm.com/case-studies/wetrade-blockchain-fintech-trade-finance
    title: we.trade

--- abstract

This document describes prominent scenarios where enterprise systems and networks maintaining digital assets require the ability to securely transfer assets or data to each other.

--- middle

# Introduction

{: #introduction-doc}

Business networks, built on both centralized and decentralized models, have emerged to manage cross-organization assets and workflows. The scope of such workflows and the assets they govern, as well as the set of participating organizations within a network, have been quite limited, partly for security, privacy, and scalability reasons, and partly because organizations have been reticent to moving large portions of their pre existing workflows to such networks. We see this especially in the areas of trade, finance, supply chain logistics, and property management. Yet the workflows managed by these networks are naturally interlinked in the real world, and therefore cannot afford to remain isolated from each other technologically, which would diminish the value of their assets. At the same time, a network, once built, has institutional staying power, and it is therefore impractical to assume that they will expand or merge. Interoperability is therefore an imperative in this fragmented business network ecosystem. This comes in different flavors, namely the ability to move an asset from one network to another, interlinking workflows to share asset state with proof of authenticity from one network to another, and swapping assets in different networks as part of a business transaction, as listed in the SAT Architecture Specification {{SATA}}. The purpose of this document is to describe prominent examples of these modes that have been encountered by enterprises and business consortiums and identified as challenges to be overcome. In particular, this document describes scenarios where the Secure Asset Transfer Protocol (SATP) {{SATP}} can be directly applied to solve the problem of moving digital assets across networks, for which no other canonical protocol exists in the literature.

# Terminology

{: #terminology-doc}

The following are some terminology used in the current document. We borrow terminology from {{NIST}} and {{ISO}} as much as possible, introducing new terms only when needed:

- Asset network (system): The network or system where a digital asset is utilized.

- Secure Asset Transfer Protocol (SATP): The protocol used to transfer (move) a digital asset from one network to another using gateways.

- Origin network: The current network where the digital asset is located.

- Destination network: The network to which a digital asset is to be transferred.

- Data sharing: The process, using the Asset Transfer Protocol, by which one or more units of verifiably authentic data are communicated from an Origin network to a Destination network, either voluntarily or upon request.

- Asset Transfer: A fail-safe process of moving an asset from one network to another, with the destruction of the asset in the Origin network and its recreation in the Destination network occurring as a single atomic action.

- Asset Exchange: A fail-safe process of exchanging (or swapping) assets held by a pair of owners, each asset being maintained in a different network, with the two in-network transfers occurring as a single atomic action.

# International Trade and Supply Chains

{: #trade-sc}

## Trade Finance and Logistics

{: #trade-sc-overview}

There are several real-world examples of consortium networks managing different aspects of international trade. Networks like We.Trade {{WET}}, built on Hyperledger Fabric {{HLF}}, and Marco Polo {{MP}}, built on R3 Corda {{R3C}}, manage trade finance workflows by connecting exporters, importers, and financial institutions (primarily banks). Other networks like TradeLens {{TL}}, built on Hyperledger Fabric, manage trade shipping and documentation logistics, by connecting exporters and shipping carriers. As an example, consider a system of two networks as illustrated in Figure 1: (a) a trade finance network managing letters of credit business lifecycles from application to fulfilment, and (b) a trade logistics network managing shipping consignment creation and dispatch documents like bills of lading.

~~~
      +------------+
      | Exporter’s |  +----------+              +---------------------+
      |    Bank    |  | Exporter |              |       Exporter      |
      +------------+  +----------+              +---------------------+
            | |            |                       | |              |
       3    | |    5       |    4           1      | |      2       |   4
    Approve | | Request    | Upload       Book     | |   Create     | Accept
      L/C   | | Payment    |   B/L     Consignment | | Consignment  |  B/L
            | |            |                       | |              |
            V V            V                       V V              V
    +-------------------------------+     +-------------------------------+
    |     Trade Finance Network     |     |    Trade Logistics Network    |
    +-------------------------------+     +-------------------------------+
            ˄              ˄                           ˄     ˄
       2    |              |    1               5      |     |    3
    Propose |              | Request        Dispatch   |     | Upload
      L/C   |              |   L/C         Consignment |     |   B/L
            |              |                           |     |
      +------------+  +----------+                 +-------------+
      | Importer’s |  | Importer |                 |   Carrier   |
      |    Bank    |  +----------+                 +-------------+
      +------------+
                   (a)                                   (b)
~~~
{: #trade-bill-figure}

An exporter who belongs to both systems must produce a valid bill of lading in the trade finance network to enforce a payment from the buyer to fulfil the terms of the letter of credit. But this bill, which serves as evidence of a shipping consignment’s dispatch via a carrier, lies in the other, i.e., trade logistics, network.  The two networks must therefore be interoperable in such a way that the logistics network can share a bill with the finance network along with independently verifiable proof of authenticity. Otherwise, the trade finance network’s workflow must trust that the exporter is acting in good faith and supplying genuine bills of lading, which adds insecurity. This interoperation, which involves sharing of network data, can be extrapolated to other scenarios involving the two networks. The trade logistics network can require an exporter to produce a valid letter of credit from the trade finance network before permitting a consignment record creation. Both these cross-network data sharing instances are illustrated in Figure 2.

~~~
               +----------+    1 Agree on      +----------+
               | Exporter |<------------------>| Importer |
               +----------+   Purchase Order   +----------+

      +------------+
      | Exporter’s |  +----------+              +---------------------+
      |    Bank    |  | Exporter |              |       Exporter      |
      +------------+  +----------+              +---------------------+
            | |                                    | |              |
       4    | |   12                        5      | |      7       |   9
    Approve | | Request                   Book     | |   Create     | Accept
      L/C   | |   L/C                  Consignment | | Consignment  |  B/L
            | |                                    | |              |
            | |                                    | |              |
            | |            |¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯|  | |              |
            | |            |    11 Share B/L    |  | |              |
            V V            V                    |  V V              V
    +-------------------------------+     +-------------------------------+
    |     Trade Finance Network     |     |    Trade Logistics Network    |
    +-------------------------------+     +-------------------------------+
            ˄              ˄    |               ˄      ˄     ˄
            |              |    |  6 Share L/C  |      |     |
            |              |    |_______________|      |     |
            |              |                           |     |
       3    |              |    2               10     |     |    8
    Propose |              | Request        Dispatch   |     | Upload
      L/C   |              |   L/C         Consignment |     |   B/L
            |              |                           |     |
      +------------+  +----------+                 +-------------+
      | Importer’s |  | Importer |                 |   Carrier   |
      |    Bank    |  +----------+                 +-------------+
      +------------+
~~~
{: #trade-letter-bill-figure}

Asset transfers among trade networks: In the preceding example, letters of credit and bills of lading represent portions of state of the larger export-import workflow. But these documents are also digital assets in their own rights.

A bill of lading can serve as title to the consignment of goods being shipped, and hence can be traded as a security or used as collateral against debt obligations in the financial market. Hence, Step 11 in Figure 2 may well be embodied by the transfer rather than the sharing of state of a bill so that it ceases to remain on the Trade Logistics Network ledger and instead belongs to the Seller’s Bank on the Trade Finance Network’s ledger.

A letter of credit may also assume the properties of a digital asset in certain situations. Consider the case of an importer who wishes to move their business to a different trade finance network and maintain their records on that network’s ledger. We can assume that the banks and the exporter participate in the second trade finance network as well, which exists to serve a different clientele. The importer needs to be able to move its letter of credit state to the other network and resume the trade workflow after migration. This requires the ability to transfer the letter in the form of a digital asset from one trade finance network to another.

## Tracking Food Shipments

{: #trade-sc-tracking}

The use case linking a trade finance network with a trade logistics network can be augmented by adding a food tracking network like the IBM Food Trust {{IFT}} to the mix. Such a network connects producers, suppliers, manufactures, and retailers, who participate in food supply chains. Purchase orders, like those negotiated between producers and retailers, and which are illustrated as negotiated between exporter and importers in Figure 2, are recorded in this network’s ledger. For quality control, its business workflow will track at periodic intervals the state (e.g., temperature and humidity) of containers carrying, for example, produce from farm to source port and from destination port to warehouse. The trade logistics network handles documentation and dispatch but does not track the location or condition of a consignment outside of a carrier’s purview. Clearly, these networks play complementary roles in a supply chain. The logistics network should be able to get the state and history of a container before dispatch from the food tracking network, as should the latter from the former after the carrier has delivered a consignment. End-to-end supply chain visibility and effectiveness relies on the interoperability of these two networks, or to be precise, their ability to share verifiably authentic data with each other. Further, such interoperation also enables the trade finance network to allow the creation of a letter of credit only after verifying the existence of a valid purchase order in the food tracking network. Figure 3 illustrates the links between these networks.

~~~
                      +-------------------------------+
                 |¯¯¯¯|     Food Tracking Network     |¯¯¯¯¯¯¯¯¯¯|
                 |    +-------------------------------+          |
         Share   |                              ˄                |  Share
        Purchase |                              |  Share         | Shipment
         Order   |         |¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯|   | Shipment       |  State
                 |         |   Share B/L    |   |  State         |
                 V         V                |   |                V
    +-------------------------------+     +-------------------------------+
    |     Trade Finance Network     |     |    Trade Logistics Network    |
    +-------------------------------+     +-------------------------------+
                                |               ˄
                                |   Share L/C   |
                                |_______________|
~~~
{: #food-tracking-figure}

## Supply Chain Management

{: #trade-sc-management}

To complete the picture, we can add a payment network to the mix, which maintains currency accounts for clients in different countries and enables cross-border payments, an example being the Stellar network {{STN}}. After goods have been dispatched, and optionally after verification of the delivery and proper condition of a shipment, payment is due from an importer to an exporter. The trade finance network can record a payment obligation on its ledger but it will rely on the payment network to process and confirm the actual transfer of funds. The former shares data about the obligation to the latter, which shares data about a successful (or otherwise) payment in return, as illustrated in Figure 4.

~~~
                      +-------------------------------+
                 |¯¯¯¯|     Food Tracking Network     |¯¯¯¯¯¯¯¯¯¯|
                 |    +-------------------------------+          |
         Share   |                              ˄                |  Share
        Purchase |                              |  Share         | Shipment
         Order   |         |¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯|   | Shipment       |  State
                 |         |   Share B/L    |   |  State         |
                 V         V                |   |                V
    +-------------------------------+     +-------------------------------+
    |     Trade Finance Network     |     |    Trade Logistics Network    |
    +-------------------------------+     +-------------------------------+
                | ˄               |               ˄
        Share   | |   Share       |   Share L/C   |
       Payment  | |  Payment      |_______________|
     Obligation | | Fulfilment
                | |
                V |
      +---------------------+
      |   Payment Network   |
      +---------------------+
~~~
{: #supply-chain-figure}

Addendum: we can add yet another network to the mix, one that manages regulatory compliance. (E.g., proof-of-concept systems have been built to bring banks and corporations on a single distributed ledger and smart contract platform to share KYC information in privacy-preserving ways {{BKYC}} {{SKYC}}.) Now issuances of letters of credit in the trade finance system will be dependent on valid KYC records being maintained as assets in the regulatory compliance system.

# Currency and Finance

{: #finance-currency}

The emerging paradigm of Decentralized Finance (DeFi) and the emerging application of Central Bank Digital Currency (CBDC) have opened up a spectrum of scenarios that require management of financial digital assets across multiple systems, typically built on distributed ledgers.

DeFi is a “new financial paradigm that leverages distributed ledger technologies to offer services such as lending, investing, or exchanging cryptoassets without relying on a traditional centralized intermediary” {{BISDeFi}}. Following the Web3 philosophy {{Web3}}, scoped for the world of finance, DeFi offers architecture and protocols built on smart contracts deployed on blockchain or other distributed ledger technology. It thereby obviates the need for centralized management and orchestration of financial processes (e.g., currency transfers, exchanges, securities settlements) by trusted authorities who can gain undue leverage.

CBDC is a form of tokenized cryptocurrency that various central banks around the world are experimenting with as the digital equivalent of traditional central bank-issued money used by banks and other financial institutions as well as end users for commercial transactions and settlements. Central banks possess exclusive authority to mint and issue money in physical cash form and in the form of electronic reserves. They also support commercial bank money used in retail transactions by banks and other users in their private capacities. Central banks have traditionally used their control over these different forms of money to enforce monetary policy in a way that promotes financial stability and provides broad access to safe and efficient payments {{BISCBDC}}. CBDCs would form a new, or alternative, type of central bank money, typically (but not always) built on blockchain or other distributed ledger technology. They have recently garnered significant interest in government circles by promising increased access and inclusion, better resilience, and increased scale and efficiency of currency transfers, compared to traditional forms of central bank-issued or central bank-backed currency.

CBDCs can broadly be classified into “wholesale” and “retail”. Wholesale CBDC, which facilitates inter-bank and cross-border settlements, is currency that is available only to banks and other financial institutions. Retail CBDC is available to the public and can be used as a digital form of cash, enabling fast transparent payments for goods and services at high scale and volume; in effect, it can be used as a substitute for legacy payment mechanisms.

Different system architectures exist to manage CBDC for banks and end users, from issuance to transfers to redemptions. A 2-tier model as illustrated in Figure 5 has recently gained popularity, where wholesale CBDC networks manage interactions between central and commercial banks, and retail CBDC networks manage interactions between commercial banks and end users. If we consider the role of the central bank as the defining characteristic of a system architecture, this model can be referred to as “indirect”, because commercial banks mediate claims between the central bank and end users and also facilitate payments. Other architectures also exist, including “direct CBDC”, where the central bank issues CBDC directly to end users and facilitates payments, and “hybrid CBDC”, which provides users the facility to make direct claims on the central bank while allowing intermediaries to facilitate payments {{BISRCBDC}}.

## Currency Transfers

{: #finance-currency-transfers}

The 2-tier “indirect CBDC” model illustrated in Figure 5 presents unique interoperability challenges that require protocols for asset transfers and which SATP is well-suited to handle. In the higher tier lie wholesale CBDC networks, bringing together central or reserve banks and various commercial banks. Following the DeFi logic, these networks are typically built on distributed ledger and smart contract technologies. Commercial banks hold reserve currency deposits with the reserve bank, which has the special power to mint currency and issue CBDC and also enforce regulatory compliance. In the lower tier lie retail CBDC networks for commercial banks and their customers, built on similar technologies, enabling seamless, efficient, and transparent payments using CBDCs. A retail CBDC network may involve a single commercial bank or multiple commercial banks, depending on the market caps of those banks and their purposes for joining such a network.

~~~
                  +----------------------------------------+
                  |                                        |
                  |         Wholesale CBDC Network         |
                  |                                        |
                  |           +----------------+           |
                  |           |  Central Bank  |           |
                  |           +----------------+           |
                  |                                        |
                  |  +------------+  +------------+        |
                  |  | Commercial |  | Commercial |        |
                  |  |  Bank A’s  |  |  Bank B’s  | ...... |
                  |  |   Account  |  |   Account  |        |
                  |  +------------+  +------------+        |
                  |                                        |
                  +----------------------------------------+
                        ˄                      ˄
                        |                      |
                        |                      |
                        V                      V
   +----------------------------+  +----------------------------+
   |                            |  |                            |
   |    Retail CBDC Network     |  |    Retail CBDC Network     |
   |                            |  |                            |
   | +------------+ +---------+ |  | +------------+ +---------+ |
   | | Commercial | | Central | |  | | Commercial | | Central | |
   | |  Bank A’s  | |  Bank   | |  | |  Bank B’s  | |  Bank   | |
   | |   Account  | +---------+ |  | |   Account  | +---------+ |
   | +------------+             |  | +------------+             |
   |                            |  |                            | .......
   | +----------------+         |  | +------------+             |
   | | Client Account | ....... |  | | Commercial |             |
   | +----------------+         |  | |  Bank C’s  |             |
   |                            |  | |   Account  |             |
   +----------------------------+  | +------------+             |
                                   |                            |
                                   | +----------------+         |
                                   | | Client Account | ....... |
                                   | +----------------+         |
                                   |                            |
                                   +----------------------------+
~~~
{: #cbdc-transfer-figure}

Here we will encounter scenarios where a given commercial bank maintains digital currency accounts in a wholesale CBDC network as well as one or more retail CBDC networks. To inject liquidity into a retail CBDC network, this bank will need to transfer currency from its reserve account in the wholesale CBDC network. Or it may need to approve (or at least audit) the transfer of currency from one retail CBDC network to another bank in another retail CBDC network. In the world of decentralized finance, or DeFi for short, currency cannot afford to remain siloed in any single CBDC network. Hence, these networks must be interoperable in order to facilitate secure transfers of currency among themselves, as illustrated in Figure 5.

We can identify two specific instances of currency transfer across networks in this example: one from a wholesale CBDC network to a retail CBDC network, and another from one retail CBDC network to another. Since currency in tokenized form is a digital asset, these scenarios require the direct application of a secure protocol for asset transfer. SATP {{SATP}} fits the bill, is agnostic of the types of distributed ledger technologies on which the respective networks are built, and simply requires the networks to use SATP gateways. This is not just a theoretical proposition; a candidate design for a bridge between Hyperledger Fabric {{HLF}} and Hyperledger Besu {{HLB}} networks using SATP and the Hyperledger Cacti interoperability platform {{HLC}} has been proposed by distributed ledger researchers {{Aug23}}.

## Multi-CBDC Economy

{: #finance-currency-multi-cbdc}

Several governments, banks and financial communities have explored the use of a shared ledger containing multiple CBDCs as way to potentially obtain an economy of scale in the development and maintenance of their own respective CBDCs. Such a Multi-CBDC approach has the potential benefit to improve cross-border payments and protect monetary sovereignty, without necessarily becoming a monetary union {{BISMCBDC}}.

However, even within a Multi-CBDC configuration, there must be a mechanism to interconnect each respective national (sovereign) bank network with the shared Multi-CBDC network. Gateways appear to be an attractive means to permit the transfer of a CBDC from one national network/ledger into the shared Multi-CBDC ledger, and vice versa.  One major requirement is the assurance that consistency is maintained between the CBDC counts on the national network with that on the Multi-CBDC network (i.e. no counterfeiting; no double-spend).

With or without a Multi-CBDC ledger, the existence of different national networks managing different wholesale CBDC assets will necessitate inter-network transfers for cross-border payments and settlements {{BISCBP}} {{WBGCBP}} {{PUbin}}. Whether directly between two wholesale CBDC networks or between a wholesale CBDC network and the Multi-CBDC network, transfer of currency assets is a problem for which SATP appears to be the most suitable solution.

## Delivery vs Payment (DvP) of Securities

{: #finance-currency-dvp}

In Decentralized Finance, or DeFi for short, investors and financial institutions will form networks to manage the creation and purchase of securities. As a simple example, we can consider a network consisting of the Treasury, which issues bonds, and commercial banks, which purchase and trade bonds. We can also consider a payment network of the kind we saw in Section 3.3 (or a retail CBDC network of the kind we saw in Section 4.1), which allows CBDC transfers between commercial banks’ accounts. In the securities network, banks may wish to transfer bonds to each other but only in exchange for compensation. But such compensation can be made only on a payment network where the two maintain currency accounts (e.g., in CBDC). Therefore, the securities and payment networks must be able to interoperate in such a way that two banks can carry out a delivery-vs-payment transaction spanning these two independent networks. Such a transaction must be atomic, i.e., either both bond and CBDC tokens get transferred in their respective networks or neither gets transferred. Figure 6 illustrates this exchange.

~~~
   +-----------------------------------------------------------------------+
   |                             Bond Network                              |
   |                                                                       |
   |     +----------+      Issue        +---------------------------+      |
   |     | Treasury |------------------>|    Commercial Bank A’s    |      |
   |     +----------+       Bond        |         Portfolio         |      |
   |                                    +---------------------------+      |
   |                                                  |                    |
   |                                                  |  Transfer          |
   |                                                  |    Bond            |
   |                                                  V                    |
   |                                    +---------------------------+      |
   |                                    |    Commercial Bank B’s    |      |
   |                                    |         Portfolio         |      |
   |                                    +---------------------------+      |
   +-----------------------------------------------------------------------+
                                       ˄
                                       |
                                       |
                                       V
   +-----------------------------------------------------------------------+
   |                 Payment Network / Retail CBDC Network                 |
   |                                                                       |
   |     +-----------+                  +---------------------------+      |
   |     |  Central  |                  |    Commercial Bank A’s    |      |
   |     |    Bank   |                  |           Account         |      |
   |     +-----------+                  +---------------------------+      |
   |                                                  |                    |
   |                                                  |  Transfer          |
   |                                                  |  Currency          |
   |                                                  V                    |
   |                                    +---------------------------+      |
   |                                    |    Commercial Bank B’s    |      |
   |                                    |          Account          |      |
   |                                    +---------------------------+      |
   +-----------------------------------------------------------------------+
~~~
{: #securities-dvp-figure}

In a variation of this example, the two commercial banks may hold CBDC accounts in two different Payment Networks. In that case, fulfilment of the DvP would require transfer of CBDC from one network to another. An instance of SATP between gateways representing those two networks would handle that problem.

## Stock Options Contract Fulfilment

{: #finance-currency-stock-options}

Stock options are financial instruments that allow holders to buy or sell stock at predetermined prices until specific expiration dates {{StOpt}}. Exercising an option, i.e., buying or selling a stock by paying a “strike price”, involves a more complex cross-network financial transaction than the securities DvP use case. Option contracts can be managed and enforced in a specific business network (which we can label as a “stock network”) to which entities like an Options Clearing Corporation (OCC), stock exchanges (e.g., the Chicago Board Options Exchange), and brokerage firms, belong. The OCC is the issuer and guarantor for all options and futures contracts traded on U.S. exchanges {{OCC}}. It provides secured back-end clearing services, while exchanges provide front-end trading markets. Transfer and settlement of payments, just like in the DvP scenario, will typically occur in a dedicated payment network in which buyers and sellers of stock have currency accounts. Options contract fulfilment requires the stock and payment networks to work in concert, and hence need SATP to coordinate transactions across them.

Figure 7 illustrates a simplified flow for the exercising of a “call” option, where a buyer acquires stock from a seller by paying it a strike price. First, the buyer informs its brokerage, which then notifies its exchange about the buyer's intent to exercise the option. The exchange in turn notifies the OCC in the Stock Network. (All these notifications typically occur via a smart contract). Steps 1-2 illustrate these notifications. The OCC then verifies the contract’s validity and the buyer’s right to exercise the option. If this is successful, the OCC triggers a payment request to the buyer through a contract-to-contract communication from the Stock Network to the Payment Network (step 3). (Alternatively, the buyer may trigger a payment request in the Payment Network, which then requests the Stock Network for proof of the contract’s validity from the OCC before approving the payment.) The buyer then pays the strike price to the seller (step 4). The payment receipt is now sent to the Stock Network for the OCC’s verification (or alternatively, the buyer can request the OCC to fetch and verify the receipt from the Payment Network) and fulfilment of the contract (step 5). The OCC, via the exchange, requests the brokerage to transfer stock from the seller’s to the buyer’s account (steps 6-7).

This cross-network transactions require SATP using gateways, either to communicate information of a contract’s validity (step 3) or a payment receipt (step 5) with authenticity proof (i.e., data sharing), or by ensuring that strike price payment (step 4) and contract fulfilment (step 6-7) occur atomically as an exchange using a coordinated set of commitments.

~~~
   +-----------------------------------------------------------------------+
   | Stock Network                                                         |
   |                                                                       |
   | +-------------+          +--------------+           +---------------+ |
   | |  Brokerage  |          |   Exchange   | 2         |      OCC      | |
   | |             |          |              | Request   |               | |
   | | +---------+ | 1        | +----------+ | to        | +-----------+ | |
   | | | Buyer   | | Exercise | |          | | Clear     | |           | | |
   | | | Equity  |-|----------|>|          |-|-----------|>|           | | |
   | | | Account | |          | | Options  | |           | | Options   | | |
   | | +---------+ |          | | Contract | |           | | Contract  | | |
   | |             |          | | (Copy)   | |           | | (Primary) | | |
   | | +---------+ |          | |          | |           | |           | | |
   | | | Seller  |<|----------|-|          |<|-----------|-|           | | |
   | | | Equity  | | 7        | +----------+ | 6         | +-----------+ | |
   | | | Account | | Fulfil & |              | Fulfil &  |               | |
   | | +---------+ | Transfer |              | Transfer  |               | |
   | |             | Stock    |              | Stock     |               | |
   | +-------------+          +--------------+           +---------------+ |
   |                                                                       |
   +-----------------------------------------------------------------------+
                           |                    ˄
          3 Request to Pay |                    |
            Strike Price   |                    |  5 Send Payment Receipt
                           |                    |
                           V                    |
   +-----------------------------------------------------------------------+
   | Payment Network                                                       |
   |                                                                       |
   |      +--------------+                           +--------------+      |
   |      |   Buyer      |    4 Pay Strike Price     |   Seller     |      |
   |      |   Payment    |-------------------------->|   Payment    |      |
   |      |   Account    |                           |   Account    |      |
   |      +--------------+                           +--------------+      |
   |                                                                       |
   +-----------------------------------------------------------------------+
~~~
{: #stock-options-contract-figure}

# Decentralized Commerce: Payments for Goods and Services

{: #decentralized-commerce}

In the emerging Web3 world, undergirded by blockchain and DLT, goods and services are increasingly available on decentralized networks, either as purely digital objects or proxies of physical objects. The networks typically manage these assets in the form of non-fungible tokens (NFTs) using smart contracts and decentralized applications (DApps for short). DeFi in a Web3 ecosystem can create thriving online marketplaces where goods and services can be bought and sold across network boundaries if those networks are interoperable (i.e., assets and data can be moved or managed seamlessly across networks). SATP is a necessary requirement to enable and secure such a decentralized form of commerce.

## Transferal of Digital Art and Payments across National Borders

{: #decentralized-commerce-digital-art}

There is currently growing interest within many artist communities of developing and selling digital-only artwork, in which the artwork consists of a file in a well-known (e.g., JPEG, MPEG) format that is created by an artist. The artists seek to sell copies of the digital-only artwork on the global marketplace, allowing anyone in the world to purchase a copy and consume (e.g., display offline) the artwork at the buyer’s discretion. Currently, the most popular technological vehicle to achieve this goal is through the tokenization of the copies of the artwork coupled with digital encryption/signature technologies to transfer control (and thereby legal ownership) of the digital-only artwork to the buyer.

Although there are a number of technical and legal challenges (e.g., copyright enforcement) to completing such a sale, one key issue pertains to the sale and payment for digital-only artwork across national borders. Many nations enforce taxation upon the sale of any asset, including that of artwork generally both domestically and internationally. Thus, when the control/ownership of a tokenized digital-only artwork is transferred to a new owner in a foreign nation and payment is received, taxation must be obtained at the point-of-sale (which could be an online platform) and proof of delivery must be traceable to ensure that no taxation-avoidance occurs. A secure asset transfer protocol between systems that can be built on distributed or shared ledgers via gateways with designated legal authority is necessary to enforce governmental regulations and provide accountability.

## Payment for Streaming Services

{: #decentralized-commerce-streaming}

Streaming services like Netflix and IPTV can tap into the cryptocurrency and DeFi user markets by offering content on distributed ledger networks using smart contracts. Instead of monthly subscriptions, they can offer pay-as-you-go streaming of arbitrarily low amounts to large numbers of users on such networks. Content transfer can be backed by NFTs, which users can redeem on any video or audio playback application. Because here already exist several payment networks for unregulated (e.g., Bitcoin) and regulated (e.g., CBDC) currencies, the content networks are likely to remain independent and not involve any monetary transactions on their own ledgers, as that would create safety and regulatory issues. Content transfer in a content network can be backed by a corresponding payment in a payment network if there is a facility to transfer payment receipts from the latter to the former. This can be fulfilled through the data sharing mode of SATP, whereby knowledge of payment along with authenticity proof can be communicated across networks. Alternatively, an atomic swap of the content and the payment can occur across both networks using the asset exchange mode of SATP.

In a related example, if users wish to obtain content that is not available currently with the streaming service provider, that provider may seek and purchase that content from another distributer that is offering it on a different content network. The copyright to that content can be backed by NFTs and the secure transfer of those NFTs from one network to another will require SATP.

Though these examples show what is possible, ongoing initiatives in Europe and China are aimed at facilitating data and asset transfers. Since 2022, China has issued a series of policies and guidelines to promote the development of a nationwide data market that supports data elements' assetization, capitalization, and circulation {{CNMeas}}. A multi-layered national data infrastructure is slated be built by the end of 2029 to support transaction, transmission, and utilization, of data; telecom operators like China Mobile and China Unicom are building large- scale networks to enable data transmission {{CNDatInf}}. Design and implementation of this infrastructure will be guided by the newly established National Data Standardization Technical Committee (TC609), which will coordinate with existing data circulation standards organizations like ISO/IEC JTC 1/SC 32 and ISO/IEC JTC 1/SC 42, and reuse existing standards.

In Europe, several projects like Gaia-X {{GaiaX}} and Catena-X {{CatenaX}} aim to create secure, decentralized, and interoperable data infrastructures. Catena-X specifically targets data exchanges in automotive industry operations while Gaia-X is a more generic, EU-wide data infrastructure. The International Data Spaces Association (IDSA) produces several ISO standards like ISO/IEC AWI 20151 and ISO/IEC 23751:2022 for exchanges across data spaces {{IDSA}}. The IDSA also partners with the Eclipse Foundation to implement open-source solutions {{EclDS}} and jointly develop the Dataspace Protocol (DSP), using which data usage policies, usage contracts, and schemas can be negotiated (in the so-called "control plane") between two data-exchange gateway peers {{DSP}}. The actual post-negotiation data transfer (in the so-called "data plane") is out of scope of DSP, and here SATP can fill the gap.

# Trustworthy DNS Resource Record Migrations using an Augmented EPP

{: #dns-epp-migration}

We have seen several examples where SATP is indispensable for enabling cross-network asset and data transfer and transaction settlement. But SATP can also be used to augment an existing protocol by making it more secure, trustworthy, and efficient rather than creating an altogether new feature that preexisting technology was unable to provide. Conventional Internet architecture offers scope for such augmentation. Though highly decentralized, the Internet consists of nodes (or actors) that play critical roles in various protocols. Such protocols would benefit if the actions of these actors can be recorded and tracked on blockchain or other decentralized ledger networks. (It must be noted that the performance implications of these augmentations ought to be studied before firm recommendations are made.)

We consider the DNS architecture {{RFC1034}} {{RFC1035}}, where multiple registries and registrars may co-exist, managing DNS records for owners (registrants). For example, Verisign {{VSign}} acts as a TLD (top-level domain) registry for the “.com” namespace, and GoDaddy {{GoDaddy}} and Squarespace {{SSpace}} are registrars that can issue and sell SLDs (second- level domains) to customers (say Alice and Bob). The Extensible Provisioning Protocol (EPP) allows registrars to communicate with registries for resource record updates, including changes in domain ownership {{RFC5730}}. Consider a scenario in which Alice, who owns an SLD (say alice.com) issued by GoDaddy, wishes to transfer that SLD to Squarespace. She can submit a request to Squarespace for this purpose, following which the respective registrars (GoDaddy and Squarespace) can communicate with the registry (Verisign) using EPP to transfer the SLD between themselves. Squarespace will then reissue the domain to Alice. In a related scenario, Alice can transfer (or sell) her GoDaddy-issued domain to Bob, who uses Squarespace as a registrant.

Though EPP facilitates these resource updates and transfers, and reputed registrars offer customers these features in a usable manner, we can see that such scenarios face safety issues as they require trust and proper coordination among the participants. These issues can be mitigated by distributed ledger networks, smart contracts, and NFTs, which collectively provide a platform for safe and transparent DNS resource transfers with easy detection of non-compliance.

In such a scheme, domains (or domain names) can be monetized as NFTs or digital assets, e.g., in the form of ERC-721 {{ERC721}} tokens, a popular NFT standard in the Ethereum ecosystem {{Ethereum}}. The creation of a domain is represented by minting of an NFT and the deletion of a domain by the burning of the NFT using smart contracts whose transactions are tracked on a distributed ledger maintained by a network of entities. Registrants Alice and Bob also participate in the smart contracts and hold wallet identities, allowing them to trade assets by submitting transactions to the ledger. Registrants, registrars, and registries can engage in commercial transactions using contracts governing tokenized (and monetized) domains for the purposes of issuing and transferring domains (among owners and registrars). This provides more safety where registrars are not reputed, and allows new registrar services to emerge and build reputations. It also enables customers like Alice and Bob to sell domains to each other safely and seamlessly.

SATP is crucial to enabling this scheme where registrars belong to, and issue, NFT-backed domains in different ledgers maintained by different networks. Ensuring that tokens are securely and atomically transferred between the ledgers will be a necessary prerequisite for an EPP resource record update operation. Further, non-compliance, or non-fulfilment of EPP, by either registrar, can be easily detected by examining the SATP logs from the respective networks’ gateways, thereby safeguarding the process. In future, reputed registrars may require their counterparties to comply with SATP-based transfers across ledgers as a prerequisite to engaging in a domain transfer with them.

This scenario additionally illustrates an example of what typically occurs in Stage 0 of a SATP instance {{SATP}}, which is where negotiation and agreement-building occurs between gateways. EPP instances among registrars and registries will occur in this stage, both prior to the start of an SATP instance and after its conclusion. EPP will produce the transaction context the gateways need to transfer an asset (in this case, a tokenized domain) using SATP. Many other applications of SATP for asset transfers may similarly augment or bolster pre-existing business workflows, which (like EPP here) will produce transactions contexts for SATP instances.

# Interoperation Protocol Considerations

{: #interop-protocol-considerations}

The use cases provided as examples serve to illustrate instances of general phenomena that the Secure Asset Transfer Protocol {{SATP}}, with a limited number of variations, is designed to handle. The data sharing examples in Section 3 can be extrapolated to any kinds of data that need to be shared between networks running arbitrary workflows. The asset transfer example in Section 4.1 and the asset exchange example in Section 4.3 similarly can be extrapolated to any kinds of digital assets lying within any kind of network. Considerations for the interoperability protocol, or SATP, can therefore be limited to standard distributed systems issues like integrity, fault tolerance, and liveness, while completely disregarding the nature of the assets, networks, and workflows, which can all remain opaque to the protocol.

# IANA Considerations

{: #satp-iana-considerations}

This document has no IANA actions.

# Contributors

{: #satp-usecases-contributors}

The authors would like to thank André Augusto of INESC-ID and Técnico Lisboa (Portugal), Zainan Victor Zhou of Namefi by D3Serve Labs, and Hyojin Song of Seoul National University (South Korea) for reviewing this draft, helping us improve its quality, and inspiring use cases in the areas of CBDC and DNS record maintenance, which augmented the existing use cases to show more applications for the interoperability modes listed in the SATP Architecture document.


--- back
