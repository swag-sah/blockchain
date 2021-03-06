---

copyright:
  years: 2017
lastupdated: "2017-07-19"
---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:pre: .pre}


# Disclaimer
{: #etn_overview}

**ATTENTION:** You must review the following information before using any {{site.data.keyword.blockchainfull}} plans.

## IBM support statement

IBM's long history of leadership in innovation continues with the {{site.data.keyword.blockchainfull_notm}} offering plans on {{site.data.keyword.Bluemix_notm}}. {{site.data.keyword.blockchain}} is a rapidly progressing technology that is projected to disrupt the financial industry, local and global supply chains, and logistical support in any number of business spaces. Through various early adoption programs, IBM customers and business partners have been actively driving blockchain as an industrial solution. {{site.data.keyword.blockchainfull_notm}} on {{site.data.keyword.Bluemix_notm}} is one such program. **As with any new technology, {{site.data.keyword.blockchainfull_notm}} on {{site.data.keyword.Bluemix_notm}} users should be aware of the potential for rapid and fundamental change**.  
{:shortdesc}

The architecture behind {{site.data.keyword.blockchainfull_notm}} is the Linux Foundation's Hyperledger Fabric project. Each open source community contribution improves Hyperledger Fabric but can present adoption challenges. **IBM cautions against defining or exchanging financial assets, or any assets of value, directly on any Hyperledger Fabric blockchain network**.  

## Open source statement

{{site.data.keyword.blockchainfull_notm}} offering plans on {{site.data.keyword.Bluemix_notm}} are built on top of the Linux Foundation's Hyperledger Fabric V1.0 stack. Hyperledger Project members, including IBM, continue to contribute to various sub-projects under the Hyperledger umbrella.  All contributions are reviewed, vetted, and tested by the community. 

Hyperledger Fabric announced it had reached *Production Level Status* for V1.0 on July 11, 2017. 

## Chaincode support statement

The following coding practices are NOT supported on {{site.data.keyword.blockchainfull_notm}} networks:

1. Using associative arrays with iteration (the order is randomized in Go).
2. Reading a list of items from a KVS table (the order is not guaranteed).
3. Writing thread-unsafe chaincode (query and invoke may be called in parallel).
4. Substituting global memory or cache storage for ledger state variables in chaincode.
5. Accessing external services, such as databases, directly from chaincode.
6. Using libraries or global variables that could introduce non-determinism (such as using "random" or "time").  

In addition, it is not recommended to write non-deterministic chaincode, which introduces risk to data consistency and integrity.  It should be noted that the Hyperledger Fabric architecture is designed to counter against non-deterministic chaincode through a series of endorsement and validation checks, however you are still strongly encouraged to code deterministic functions that are not reliant on non-static global variables (e.g. time).  
