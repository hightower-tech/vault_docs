# Concept

In VAULT Wallet, the user is provided with an EVM-compatible address during registration, which acts as an abstraction of their account. This account is created using ZeroDev, a powerful infrastructure provider that specializes in Account Abstraction. At the core of Account Abstraction lies the concept of the smart account—an account that is powered by a smart contract, rather than the traditional externally owned account (EOA) used in blockchain networks.

The VAULT Wallet leverages the modular design of **Kernel**, a smart account solution that can be extensively customized using plugins. This modular approach allows for a flexible architecture that meets the diverse needs of users while maintaining a secure foundation. Kernel enables smart accounts to integrate various functionalities in a plug-and-play manner, offering a highly customizable user experience.

[Kernel smart-contracts on GitHub](https://github.com/zerodevapp/kernel)

### **Permissioned Key Management**

One of the standout features of Kernel is its approach to key management. With Kernel, different permissions can be assigned to different keys, offering a sophisticated level of access control for smart accounts. These keys fall into two main categories:

1. **Owner Keys**: These are keys owned by the user, or potentially by multiple co-owners, providing full control over the smart account. They enable the owner to execute any transaction, manage plugins, and configure settings.
2. **Session Keys**: These are short-lived keys designed to delegate limited permissions to others, such as for executing specific types of transactions or interacting with a dApp. The concept of session keys introduces a new level of flexibility, allowing users to delegate functionality without exposing full account control. This is especially useful in scenarios where trust is partial or temporary, such as allowing a third-party service to make transactions for a limited period.

### **Account Customization via Plugins**

Plugins play a key role in enhancing the functionality of smart accounts. Through the use of plugins, the VAULT Wallet can integrate a wide range of features directly into the user's account. This can include advanced security configurations, automated transaction logic, spending limits, or integrations with DeFi protocols. The modularity provided by Kernel allows for continuous improvement and the ability to tailor user experiences to specific needs without redeploying the entire smart contract.

For example, a user could add a plugin that limits transaction spending per day or automatically invests excess stablecoins into a yield-generating DeFi protocol. The flexibility of plugins ensures that the VAULT Wallet can cater to different user profiles—whether they are casual users, power users, or institutional participants.

### **Enhanced Security Model**

The combination of owner keys and session keys provides a security model that is both robust and user-friendly. Users can assign different keys to different actions, which helps mitigate risks related to key compromise. Session keys, in particular, provide a convenient way to authorize third parties for limited actions, without putting the entire account at risk. This makes the system suitable for use cases such as gaming, DeFi, and social applications, where users may need to interact with smart contracts regularly but require an added layer of security.

By utilizing ZeroDev and Kernel, the VAULT Wallet ensures that account management is seamless, secure, and flexible, removing traditional barriers of interaction within the Web3 ecosystem. This allows users to engage in cross-network stablecoin transfers and other blockchain activities without the complexity typically associated with decentralized finance.
