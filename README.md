# NFT-anti-hack-checklist

NFTs have exploded in popularity in the last year because of their unique ability to assign value to any digital or physical object while recording ownership in the Blockchain.
The recent rise in popularity of these NFTs is due to a lack of information available both offline and online, making them a popular target for scammers and hackers.

In this repository, we have created a checklist for developers as well as for users to prevent these hacks/scams and stay safe from these hackers/scammers.

**If you find anything missing or want to update existing resources, you can create a pull request and contribute to the project.**

## Security Measures for Developers:


| Serial No | Topic | Description |
| --- | --- | --- |
| 1 | **After Deployment, Transfer Ownership to the Multisig** |When deploying contracts, your NFT contract has the wallet address you used to deploy it set as its current owner. Multisig ownership is more secure, we should transfer ownership to the multisig created earlier after deployment. |
| 2 | **Use the latest version of Solidity/Rust** | When deploying NFTs, use the most recent version of Solidity/Rust. This is due to the regularity with which breaking updates, new features, and bug fixes are introduced. Check that your code has no reported issues with the latest compiler version. |
| 3 | **Hire experienced developers** | To ensure you develop the best NFT project out there, make sure to hire a developer who is skilled and experienced. |
| 4 | **Full unit test coverage** | Unit testing improves software quality with every code check-in and build. Unit testing is the quickest, most direct way to identify and fix bugs before they influence the main codebase.
| 5 | **Follow well-known programming practices** | Smart contracts are developed using different programming languages, such as Solidity, Vyper, Rust, etc. The development of smart contracts has proven to be extremely error-prone. It is important to follow best programming practices to develop secure NFT. |
| 6 | **Log all crucial operations** | Events will aid in contract debugging during development and contract monitoring after deployment. So, It is recommended to emit events for critical functions like changing owners, minting, burning tokens, etc. |
| 7 | **Use the latest and well-tested libraries** | Always use the latest and well-tested libraries like openzeppelin. These libraries are well tested, and community-reviewed contracts, so they are considered more secure. For example, If we want to write an NFT contract, we can use OpenZeppelin's ERC721 Library. See here for [more](https://docs.openzeppelin.com/contracts/4.x/erc721) details. |
| 8 | **Avoid known pitfalls and common NFT vulnerabilities** | Learn the most pitfalls and common security vulnerabilities in NFT contracts and how to mitigate them. Watch out for common bugs like Reentrancy, Denial of Service, etc. Do check out [NFT Attack Vectors](https://github.com/Quillhash/NFT-Attack-Vectors) which contains a  complete list of NFT Attacks. |
| 9 | **Access Control Protection for critical operations** | Hackers can easily exploit an NFT contract if access control is handled poorly or not at all. So, the protocol needs to implement access control protection and restrict critical functions like changing owners, pausing contracts, etc. to the owner/admin role. |
| 10 | **Always list NFTs in a Reputable and secure marketplace** | Try to list your NFTs in a more secure NFT Marketplace, as there have been many incidents in the past of NFT marketplace vulnerability leading to stealing users' NFTs. So, choose NFT Marketplace wisely. |
| 11 | **NFT audits** | Audit will help us detect uneven and unexpected vulnerabilities of NFT projects before deployment and, therefore, ensure security.
| 12 | **Bug bounty program** | Projects can host their bug bounty program or integrate with Bug Bounty Platforms like Immunefi or Hackerone. It adds an extra layer of security for the projects. |
| 13 | **Safeguard wallet of Admin/Owner** | The Admin role is used to manage upgrades and various privileges role in logic. If the private key of the admin/owner of an NFT contract is leaked, the entire NFT project may be destroyed. So, Properly secure your wallet and always use a hardware wallet or a multisig wallet which is considered more secure. Check out this [blog](https://blog.trailofbits.com/2018/11/27/10-rules-for-the-secure-use-of-cryptocurrency-hardware-wallets/) for more details on wallet security. |
| 14 | **Enable Authentication Methods/ 2FA to prevent Social account hacks.** | There are lots of scenarios where these NFT projects' social media accounts like Discord and Twitter are hacked, and the hackers use the compromised accounts for their gain. Check out this [blog](https://medium.com/quillhash/analysing-nfts-discord-server-hacks-quillaudits-46f8d874f913) for more details on NFT social media hacks and their prevention methods.
| 15 | **Add checks for Weak Random Number Generation** | The weak PRNG issue is way too common in the NFT gaming ecosystem. It is recommended to use Chainlink VRF for generating a PRNG. Never use predefined methods related to the block like block.timestamp, block.number, or a controlled user input for generating random numbers. 

---


## Safety Tips For Users:

| Serial No | Topic | Description |
| --- | --- | --- |
| 1 | **Only trade on reputable NFT marketplaces** | Security is an important consideration for many NFT traders, especially given there have already been several high-profile platform hacks. So, try to trade at a reputable and secure nft marketplace.
| 2 | **Use two-factor authentication to add an extra layer of security to your crypto wallet.** | Try using two-factor authentication (2FA) wherever possible. This is one of the strongest forms of authentication, as hackers would need to have your password and access your mobile phone to log into your wallet. The best way to store your NFTs is through a hardware wallet since it’s offline.
| 3 | **Regularly back up your wallet** | A backup of your wallet can protect you from computer problems as well as many human errors. If you keep your wallet encrypted, you may be able to recover it if your phone or computer is destroyed.
| 4 | **Never blind-sign NFT transactions** | Before confirming the transaction, always examine the permission details in the smart contracts. Many hackers disguise their actions in smart contracts, giving them unauthorized access to funds in your wallet. If possible try to read the smart contract details carefully and validate that they do not provide a threat or vulnerability.
| 5 | **Research well before you invest** | There have been many incidents in the past where the NFT team abandons their project and disappears with the money raised from investors. So, before investing in an NFT initiative, conduct your research. Before investing, research the project founders' profiles and backgrounds.
| 6 | **Always review your token approvals & revoke unused ones** | Every day, we engage with various protocols and links, granting them access and permission depending on the information in the smart contract. It is critical to periodically check and revoke access and permissions granted. You can use [revoke.cash](https://revoke.cash) to cancel access.
| 7 | **Download web3 apps or wallets from official websites** | One of the biggest causes of crypto/NFT hacks is that users access unofficial sites which always look like the official website. Hackers usually use this to embed their malicious contract and once you sign the transaction, they can steal all your nfts/tokens.
| 8 | **Only interact with official channels, Twitter accounts, and links** | Always restrict your telegram, discord, and email from receiving messages from strangers and unofficial addresses. Use a [link-checking](https://www.makeuseof.com/tag/4-quick-sites-that-let-you-check-if-links-are-safe/) website first, which will let you know if a site is legitimate or not.
| 9 | **Never share your seed phrase or wallet private key with anyone** | If you reveal your seed phrase or private keys with anyone, they will have access to your digital assets. Anyone who has access to your private key/seed phrase can steal all of your tokens and NFT.
| 10 | **Regularly update your device/software and Protect them with cybersecurity software** | It is easy to encounter malware, spyware, and other malicious software while browsing online. So, it is important to protect your device and data using security software like anti-virus and VPNs for more security.

---

### References:
https://web3caff.com/archives/9629   
https://merehead.com/blog/make-nfts-secure/
