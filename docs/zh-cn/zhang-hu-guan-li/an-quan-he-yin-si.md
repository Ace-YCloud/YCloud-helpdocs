---
doc_id: doc_zhang_hu_guan_li_an_quan_he_yin_si
language: zh-CN
title: "安全和隐私"
slug: an-quan-he-yin-si
path: zhang-hu-guan-li/an-quan-he-yin-si
document_group: zhang-hu-guan-li
path_in_group: an-quan-he-yin-si
parent_id: doc_zhang_hu_guan_li
order: 990
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:20:37.675Z
updated_at: 2026-04-02T11:20:37.675Z
last_synced_at: 2026-04-02T11:20:37.675Z
tags:
---

# 安全和隐私

在 YCloud, 保护客户隐私和数据安全是我们的不变承诺。我们以严谨的态度对待每一个可能影响您的细节，凭借专业的团队和完善的机制，为您的数据安全和隐私保护筑起坚不可摧的防线。

## 安全策略设计

YCloud采用纵深防御方法，在整个组织中实施多层安全措施。我们的安全策略不仅受合规和监管要求的驱动，还受行业最佳实践的驱动，如OWASP Top 10和CIS关键安全控制和威胁情报。目前仍在不断完善我们现有的安全控制。

## **数据安全**

YCloud使用多种DataStore来存储数据并确保数据安全。每个DataStore的配置都遵循数据安全和恢复的最佳实践。

当平台中的数据被复制到多个服务集群。如果一个服务集群的服务器出现故障，处理将切换到另一个服务集群的备用服务器，最小化服务中断影响。

我们的灾难恢复策略使用数据快照和每日完整备份的组合，以确保有多个数据副本可供恢复。快照旨在提供快速恢复机制，恢复可以在几分钟内完成。当快照无法恢复数据时，使用完整备份。

## **通信安全**

Web客户端和YCloud服务器之间的所有通信都使用强密码套件的TLS（1.0、1.1、1.2）协议加密进行保护。

YCloud的所有页面均通过HTTPS安全加载。

## **系统可靠性**

YCloud使用的微服务架构中的每项服务都分布在不同数据中心运行的多个服务器上。这些服务使用API相互通信，以减少彼此之间的相互依赖关系。我们每次更新在部署之前都会在相应的测试环境进行测试。

YCloud还利用全球内容交付网络（CDN）将内容分发到离用户最近的位置，无论您身在何处，都可以快速一致地访问。

## **基础设施安全**

我们利用HIDS、 WAF 等安全产品来确保您的数据安全。让您的信息受到顶级基础设施安全措施的保护。



其他相关内容敬请查看：

[服务条款](https://www.ycloud.com/terms-service)

[隐私条款 ](https://www.ycloud.com/privacy-policy)

[Shopify店铺隐私协议](https://www.ycloud.com/sp-policy)
