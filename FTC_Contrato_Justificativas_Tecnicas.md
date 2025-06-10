
# FTC – Justificativas Técnicas de Segurança do Contrato

Esta seção tem como objetivo esclarecer os pontos levantados por ferramentas automatizadas de análise, como o TokenSniffer, e demonstrar a transparência e segurança do contrato da FinTech Coin (FTC).

---

## 🔍 Análise de Segurança

### ✅ Token Vendável
O contrato da FTC foi analisado por mecanismos como o TokenSniffer e Honeypot.is. O resultado indica que o token **é vendável**, ou seja, **não é um honeypot**.

---

### 🔸 Pausable Contract
Utilizamos o módulo `Pausable` da biblioteca OpenZeppelin como medida de **segurança preventiva** para cenários críticos.
- Esta função **nunca foi ativada** e está desabilitada por padrão.
- Transparência total: essa proteção serve apenas para pausas emergenciais, se necessário.

---

### 🔸 Max Transaction Amount
O contrato possui uma função para definir um valor máximo por transação.
- **Atualmente, esta função está desativada**.
- Ela existe apenas como recurso para **prevenir manipulações iniciais de mercado**.

---

### 🔸 Ownership Não Renunciado
O controle de ownership ainda está com o deployer, **com o objetivo de realizar melhorias futuras com responsabilidade**.
- Nenhuma função de **mintagem**, **alteração de taxas**, ou **bloqueio de transferências** está ativa ou disponível.
- A comunidade será consultada antes de qualquer alteração estrutural.

---

### 🔒 Liquidez Travada
Toda a liquidez foi adicionada ao par FTC/ETH na Uniswap V3 e **100% travada via Unicrypt**, com validade até:
- **26 de novembro de 2025** (Pool 1)
- **30 de novembro de 2025** (Pool 2)

Verificável em: [Link da Unicrypt]

---

## 📌 Conclusão

Apesar dos alertas genéricos gerados por scanners automáticos, o contrato da FTC é transparente, auditável e **seguro para a comunidade**.  
Essa seção visa esclarecer dúvidas técnicas e reforçar o compromisso com a **construção de um ecossistema confiável**.

