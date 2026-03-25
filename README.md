# 🚀 Full Control 2.0 - Gestão de Semi Acabados

> Sistema avançado de controle de estoque, estrutura de produtos (BOM) e gestão de produção para a **Elka Plásticos**.

---

## 📝 Sobre o Projeto
O **Full Control 2.0** é uma solução robusta para o controle de materiais semi-acabados. Diferente de sistemas de recados, esta versão foca no **balanço de massa**: ele entende que para produzir uma "Referência", é necessário consumir várias "Peças" do estoque, automatizando a baixa e o cálculo de disponibilidade.

O sistema utiliza **Supabase (PostgreSQL)** como banco de dados em tempo real, permitindo que múltiplos usuários gerenciem o inventário simultaneamente com persistência de dados segura.

## 🛠️ Principais Funcionalidades

### 📊 Dashboard Inteligente
* **Visão Geral:** Cards com total de referências, produções do dia e alertas de estruturas (BOM) incompletas.
* **Estoque Crítico:** Listagem automática de itens abaixo do nível de segurança.
* **Linha do Tempo:** Histórico visual das últimas 25 atividades (Entradas, Saídas e Ajustes).

### 🏗️ Gestão de Estrutura (BOM - Bill of Materials)
* **Montagem de Kits:** Defina exatamente quantas peças de cada código compõem uma Referência final.
* **Cálculo de Capacidade:** O sistema analisa o estoque atual e informa instantaneamente: *"Com o que temos hoje, podemos montar X unidades da Ref. 45"*.

### 📦 Controle de Estoque e Processamento
* **Entrada de Material:** Registro de chegada de novos lotes com atualização automática do saldo.
* **Transformação (Processamento):** Módulo para registrar a passagem de peças brutas para acabadas (Tampografia, Pintura, Transfer).
* **Ajuste Rápido:** Edição direta de estoque com registro automático no histórico para auditoria.

### 🏭 Produção e Simulação
* **Baixa Automática:** Ao registrar a produção de uma referência, o sistema abate proporcionalmente todas as peças daquela estrutura no estoque.
* **Simulador de Faltas:** Ferramenta que projeta uma produção futura e gera um relatório listando exatamente o que falta comprar ou produzir.

### 📂 Importação e Exportação
* **Importação via CSV:** Cadastro em massa de referências e peças para agilizar a implantação.
* **Exportação para Excel:** Gera inventários completos e relatórios de diferenças formatados para uso administrativo.

## 🚀 Atalhos de Produtividade (Hotkey)
Para agilizar a operação no chão de fábrica, o sistema conta com atalhos de teclado:
* `ALT + 1` até `ALT + 7`: Navegação rápida entre as abas.
* `Enter`: Confirma cadastros, entradas e produções automaticamente.

## ⚙️ Tecnologias Utilizadas
* **Frontend:** HTML5, CSS3 (Flexbox/Grid), JavaScript (ES6+).
* **Backend como Serviço:** [Supabase](https://supabase.com/) (Banco de Dados Relacional).
* **Persistência:** PostgreSQL em nuvem.

## 📋 Como Configurar
1. **Banco de Dados:** Certifique-se de que as tabelas `refs`, `pecas`, `bom` e `hist` estão criadas no seu projeto Supabase.
2. **Hospedagem:** O arquivo é estático e pode ser rodado via **GitHub Pages**, Vercel ou até mesmo localmente.
3. **Segurança:** As chaves de acesso estão configuradas para o ambiente atual; para produção, recomenda-se configurar o RLS (Row Level Security) no Supabase.

---
📅 **Desenvolvedor:** [Seu Nome]  
🏢 **Foco:** Elka Plásticos - Eficiência Industrial
