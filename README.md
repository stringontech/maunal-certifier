---
description: 防伪认证系统是“区块链防伪”业务下的其中一个系统，由认证机构使用和管理。
---

# 简介

区块链防伪业务是由弦子科技专门针对防伪溯源市场所打造的防伪系统，帮助消费者识别商品真伪，防止假冒。

## 业务流程

![&#x6D41;&#x7A0B;&#x56FE;](http://md.stringon.com/img/%7Bfilename%7D%7B.suffix%7D20200904104846.png)

1. **生产码：**由防伪码认证机构借助统进行生产防伪码。
2. **制码：**生产好的码需要进行文件导出，导出后发给印刷厂进行印码。
3. **寄回：**印刷完成的码以及作废的废码文件一并寄回给防伪认证机构。
4. **激活码：**收到防伪码后商家将废码信息导入到系统内，将可用码进行激活。
5. **定义商品：**生产商首先定需要在系统内定义出需要使用防伪码的商品的商品信息，该商品信息将绑定至防伪码上。
6. **申请防伪码：**基于商品 sku 向认证机构申请使用防伪码，填写申请数量，将申请单提交到认证机构处。
7. **寄出、划拨：**认证机构审核申请单，没有问题便同意申请，并在系统内将码进行划拨给生产商，相关码进行上链记录，同时也将对应的打印码线下寄给生产商。
8. **申请授权**：某生产商可申请成为其他生产商的授权销售商，双方建立联系后授权销售商即可从生产商处拿到贴有防伪码的商品。
9. **二次划拨：**生产商将防伪码划拨给授权销售商的过程。
10. **贴码、售卖：**生产商（或授权销售商）收到码以后将码贴到商品上，并通过各种方式进行售卖，最终到用户手中。
11. **扫码、验码：**用户购买到商品后，可以通过商品上贴的防伪码进行验证，输入核验码即可进行验证。

## 业务角色说明

**认证机构**

- 认证机构是指能够发行和生产防伪码的机构，所有流通中的防伪码均是由认证机构所生成。每一个码均带有认证机构的签名信息。
- 使用系统：防伪认证系统


**生产商**

- 生产商是指能够定义和发行商品信息的人，所有流通中的商品均是由生产商所发行，由生产商向认证机构申请防伪码进行关联商品，并进行售卖。售卖出去的防伪码带有生产商的签名信息。
- 使用系统：数字工场


**授权销售商**

- 该角色为防伪业务下的特殊角色，可售卖生产商已关联完防伪码的商品，由该角色售卖的商品，防伪码会额外标有授权销售商的签名信息。
- 使用系统：数字工场


**消费者**

- 消费者指购买到贴有防伪码的商品的用户。
- 使用系统：物影钱包


## **系统说明**

**防伪认证系统**

- 用来生产、管理、划拨防伪码的系统。
- 使用角色：认证机构


**数字工场**

- 生产区块链资产的系统，围绕商品相关的业务包括定义、发行、发货、核销、防伪码等业务，均在该系统内完成。
- 使用角色：生产商、授权销售商


**物影钱包**

- 面向 C 端的一款产品，帮助用户管理自己的区块链资产。
- 使用角色：消费者


## **名词解释**

**激活**：指将防伪码从创建到可以进入使用环节的过程，激活过后的码均为可使用的码。

**作废**：因为印刷厂在印刷防伪码过程中存在一定的报废率，所以对于报废的码需要过滤掉，不可进入流通环节。

**划拨**：指将防伪码从防伪认证机构到生产商手中的过程。

**二次划拨**：指将防伪码从生产商到授权销售商手中的过程。

**归属**：每一次的划拨，都代表了当前防伪码持有权的转让，归属信息即表示谁持有了哪个码。

**核验**：消费者刮开防伪码并进行查验真伪的过程即为核验过程，核验状态表示了防伪码是否被使用过。

**三方签名**：每一个防伪码由哪些机构授权支持的签名信息，目前包括：弦子科技签名（提供技术支持）、认证机构签名（提供认证支持）、生产商签名（提供商品授权）这三个签名信息，另外若包含授权销售商，则额外还有授权销售商签名（提供销售渠道信息）。

