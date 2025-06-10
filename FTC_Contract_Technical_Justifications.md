
# FTC – Technical Justifications for Contract Security

This section aims to clarify the points raised by automated auditing tools, such as TokenSniffer, and demonstrate the transparency and safety of the FinTech Coin (FTC) contract.

---

## 🔍 Security Analysis

### ✅ Sellable Token
The FTC contract has been analyzed by tools such as TokenSniffer and Honeypot.is. The result confirms that the token **is sellable**, meaning it is **not a honeypot**.

---

### 🔸 Pausable Contract
We use the `Pausable` module from the OpenZeppelin library as a **preventive security measure** for critical scenarios.
- This function has **never been activated** and is disabled by default.
- Full transparency: this safeguard exists solely for emergency pauses, if needed.

---

### 🔸 Max Transaction Amount
The contract includes functionality to set a maximum transaction amount.
- **This function is currently disabled**.
- It exists as a precautionary tool to **prevent early market manipulation**.

---

### 🔸 Ownership Not Renounced
Ownership remains with the deployer to **responsibly enable future improvements**.
- There are no active functions for **minting**, **fee changes**, or **transfer blocking**.
- The community will be consulted before any structural changes are made.

---

### 🔒 Locked Liquidity
All liquidity was added to the FTC/ETH pair on Uniswap V3 and is **100% locked via Unicrypt**, with lock periods until:
- **November 26, 2025** (Pool 1)
- **November 30, 2025** (Pool 2)

Verifiable at: [Unicrypt Link]

---

## 📌 Conclusion

Despite the generic alerts triggered by automated scanners, the FTC contract is transparent, auditable, and **safe for the community**.  
This section aims to clarify technical doubts and reinforce our commitment to **building a trustworthy ecosystem**.

