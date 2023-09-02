# ChatModeler

## 案例1：ATM系统需求案例

### 1.1 原始需求文本

```
The bank client must be able to deposit an amount to and withdraw an

amount from his or her accounts using the bank application. Each

transaction must be recorded, and the client must have the ability to

review all transactions performed against a given account. Recorded

transactions must include the date, time, transaction type, amount and

account balance after the transaction. A bank client can have two types of

accounts: a checking-account and a saving-account. For each checking

account, one related saving-account can exist. The application must verify

that a client can gain access to his or her account by identification via a

personal identification number (PIN) code. Neither a checking-account nor

a saving-account can have a negative balance. The application should

automatically withdraw funds from a related saving account if the

requested withdrawal amount on the checking-account is more than its

current balance. If the saving-account balance is insufficient to cover the

requested withdrawal amount, the application should inform the user and

terminate the transaction
```

### 1.2 对话记录

注意：用户内容为手动输入，其他均为自动生成。

**收集者：** Hi there! What kind of system would you like to develop?

**用户：**I want to develop an ATM system. I hope the bank client can deposite an amount to and withdraw an amount from his or her accounts using this bank application.

**建模者：**Got it. From the user's response, I can extract the following requirement domain entities: Actor - <u>bank client</u>; Action - <u>deposit an amount, withdraw an amount</u>.

**检测员：**Got it! Based on the information you provided, it looks like the bank client's actions should include the ability to deposit and withdraw funds. Additionally, the bank client should have the ability to review all transaction, access to balance, and inform the user.

**收集者：**Are you looking for a system that would allow the bank client to review all transactions?

**用户：**yes, I hope the bank client can review all transaction using this system

**建模者：**Got it. From the user's response, I can extract the following requirement domain entities: Actor - bank client; Action - <u>review all transactions</u>. 

**检测员：**Got it! Based on the information you provided, it looks like the bank client's actions should include the ability to deposit and withdraw funds, as well as access to balance, and inform the user.

**收集者：**Are you looking for a system that would allow the bank client to access to balance?
**用户：** yes, I hope the bank client can access to balance.

**建模者：**Got it. From the user response, I have extracted the following requirement domain entities: Actor - bank client; Action - <u>access to balance</u>.

**检测员：**Got it! Based on the information you provided, it looks like the bank client's actions should include the ability to deposit and withdraw funds, as well as access to balance information, and inform the user.

**收集者：**Are you looking for a system that can inform the user?

**用户：**yes, the system must have the ability to inform the user.

**建模者：**Got it. From the user response, I have extracted the following requirement domain entities:  Action -  inform the user.

**检测员：**Got it! Please ask whether other actor use this system.

**收集者：** Are you looking for a system that would allow other people to use it as well?
**用户：**No, only bank client
**建模者：**Got it. From the user response, I have extracted the following requirement domain entities: Actor - bank client; Action - none.

**综上：交互次数为5**

### 1.3 建模结果

|             | 人工                                     | IT4RE                                    | GPT3.5                                   | LLama | ChatLGM |
| ----------- | -------------------------------------- | ---------------------------------------- | ---------------------------------------- | ----- | ------- |
| **Actors**： | Bank_Client                            | Application Client                       | bank_client                              |       |         |
| **Actions** | Deposit Withdraw  Review Access Inform | Cover Deposit Gain Withdraw Have Include Inform Review | deposit an amount, withdraw an amount,review all transactions,access to balance,inform the user,**transfer funds between accounts, and set up automatic payments.** |       |         |



### 1.4 需求文档

将所有的对话记录输入给大模型，加上设计的提示词模板，生成的需求文档。

```

```



## 案例1：ATM系统需求案例

### 1.1 原始需求文本

```
The bank client must be able to deposit an amount to and withdraw an

amount from his or her accounts using the bank application. Each

transaction must be recorded, and the client must have the ability to

review all transactions performed against a given account. Recorded

transactions must include the date, time, transaction type, amount and

account balance after the transaction. A bank client can have two types of

accounts: a checking-account and a saving-account. For each checking

account, one related saving-account can exist. The application must verify

that a client can gain access to his or her account by identification via a

personal identification number (PIN) code. Neither a checking-account nor

a saving-account can have a negative balance. The application should

automatically withdraw funds from a related saving account if the

requested withdrawal amount on the checking-account is more than its

current balance. If the saving-account balance is insufficient to cover the

requested withdrawal amount, the application should inform the user and

terminate the transaction
```

### 1.2 对话记录

注意：用户内容为手动输入，其他均为自动生成。

**收集者：** Hi there! What kind of system would you like to develop?

**用户：**I want to develop an ATM system. I hope the bank client can deposite an amount to and withdraw an amount from his or her accounts using this bank application.

**建模者：**Got it. From the user's response, I can extract the following requirement domain entities: Actor - <u>bank client</u>; Action - <u>deposit an amount, withdraw an amount</u>.

**检测员：**Got it! Based on the information you provided, it looks like the bank client's actions should include the ability to deposit and withdraw funds. Additionally, the bank client should have the ability to review all transaction, access to balance, and inform the user.

**收集者：**Are you looking for a system that would allow the bank client to review all transactions?

**用户：**yes, I hope the bank client can review all transaction using this system

**建模者：**Got it. From the user's response, I can extract the following requirement domain entities: Actor - bank client; Action - <u>review all transactions</u>. 

**检测员：**Got it! Based on the information you provided, it looks like the bank client's actions should include the ability to deposit and withdraw funds, as well as access to balance, and inform the user.

**收集者：**Are you looking for a system that would allow the bank client to access to balance?
**用户：** yes, I hope the bank client can access to balance.

**建模者：**Got it. From the user response, I have extracted the following requirement domain entities: Actor - bank client; Action - <u>access to balance</u>.

**检测员：**Got it! Based on the information you provided, it looks like the bank client's actions should include the ability to deposit and withdraw funds, as well as access to balance information, and inform the user.

**收集者：**Are you looking for a system that can inform the user?

**用户：**yes, the system must have the ability to inform the user.

**建模者：**Got it. From the user response, I have extracted the following requirement domain entities:  Action -  inform the user.

**检测员：**Got it! Please ask whether other actor use this system.

**收集者：** Are you looking for a system that would allow other people to use it as well?
**用户：**No, only bank client
**建模者：**Got it. From the user response, I have extracted the following requirement domain entities: Actor - bank client; Action - none.

**综上：交互次数为5**

### 1.3 建模结果

|             | 人工                                     | IT4RE                                    | GPT3.5                                   | LLama | ChatLGM |
| ----------- | -------------------------------------- | ---------------------------------------- | ---------------------------------------- | ----- | ------- |
| **Actors**： | Bank_Client                            | Application Client                       | bank_client                              |       |         |
| **Actions** | Deposit Withdraw  Review Access Inform | Cover Deposit Gain Withdraw Have Include Inform Review | deposit an amount, withdraw an amount,review all transactions,access to balance,inform the user,**transfer funds between accounts, and set up automatic payments.** |       |         |



### 1.4 需求文档

将所有的对话记录输入给大模型，加上设计的提示词模板，生成的需求文档。