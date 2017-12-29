# 《BlindBox》论文笔记

[TOC]

*原文标题《BlindBox: Deep Packet Inspection over Encrypted Traffic》*

## 摘要

### MiddleBox & DPI Intro.

网络中间件（Network MiddleBox）：*deep packet inspection*（DPI）

DPI Tasks：

- Intrusion detection(IDS)
- Exfiltration detection
- Parental filtering



### A long-standing issue

Once packets are sent over HTTPS, middleboxes can no longer accomplish their tasks because the payloads are encrypted.

 Hence, one is faced with the choice of only one of two desirable properties: the **functionality** of middle-boxes and the **privacy** of encryption.



### Solution: BlindBox

BlindBox is the first system that simultaneously provides both of these properties.

**Approach**:  perform the deep-packet inspection *directly on the encrypted traffic*.

**Realizes** this approach through: a new protocol and new encryption schemes.



### Features of BlindBox

- Enables applications like MiddleBox
- Supports real rulesets from both *open-source* and *industrial DPI systems*
- Practical for settings with long-lived HTTPS connections
- Its core encryption scheme is 3-6 orders of magnitude faster



