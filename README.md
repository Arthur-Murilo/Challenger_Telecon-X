# Challenger_Telecon-X

A evasão de clientes (Churn) é um dos principais desafios enfrentados por empresas de telecomunicações. O objetivo deste estudo é analisar os padrões de evasão dos clientes da TelecomX com base em dados reais. Compreender o comportamento de cancelamento pode ajudar a empresa a reter mais clientes e reduzir perdas financeiras.

---

## 🧼 Limpeza e Tratamento de Dados

- O conjunto de dados foi importado de uma API pública em formato JSON.
- As colunas foram padronizadas para letras minúsculas.
- Valores "Yes"/"No" foram convertidos para valores booleanos (1 e 0).
- A variável `churn` também foi transformada em 0 e 1.
- Foi criada uma nova coluna `contas_diarias` para analisar o custo médio diário do cliente.
- Valores não numéricos de `account.charges.total` foram convertidos com tratamento de erros.

---

## 📊 Análise Exploratória de Dados

- Cerca de **26% dos clientes cancelaram o serviço**, mostrando um risco significativo de evasão.
- Clientes com **contratos mensais** têm taxas de churn muito maiores que aqueles com contratos anuais ou bianuais.
- Métodos de pagamento como **fatura eletrônica** e **cartão de crédito** apresentaram maior associação com cancelamentos.
- Clientes que cancelam geralmente possuem **menor tempo de contrato (tenure)** e **gastam menos** ao longo do tempo.

---

## 💡 Conclusões e Insights

- A **fidelização aumenta** com contratos mais longos.
- É possível prever churn com base em comportamento de consumo (tempo de contrato, total gasto, etc.).
- Clientes com perfil de pagamento manual (fatura) têm maior risco de sair.
- Perfis como **usuários sem dependentes ou parceiros** também tendem a cancelar mais.

---

## ✅ Recomendações

- **Oferecer incentivos para contratos longos**, como desconto progressivo.
- **Implementar campanhas de retenção** para clientes nos primeiros meses de uso.
- **Migrar clientes para métodos de pagamento automáticos**, como débito automático.
- **Criar perfis de risco** baseados em churn para aplicar ofertas personalizadas.

---

Essa análise pode servir de base para um modelo preditivo com algoritmos de Machine Learning em etapas futuras.
