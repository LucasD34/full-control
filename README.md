# 🚀 Full Control S.A. - Gestão de Semi-Acabados

O **Full Control S.A.** é um sistema web leve e eficiente projetado para o controle de estoque e ordens de produção da **Elka Plásticos**. Ele permite gerenciar referências, componentes (BOM), entradas de materiais e o cálculo automático de capacidade produtiva.

---

## 🛠️ Funcionalidades Principais

* **Dashboard em Tempo Real:** Visualização de estoque crítico, produção do dia e últimas atividades.
* **Gestão de Estoque (BOM):** Controle detalhado de peças por referência com barras de progresso visual.
* **Cálculo de Máximo Produtivo:** O sistema indica automaticamente quantas unidades de um produto podem ser fabricadas com o estoque atual.
* **Importação via CSV:** Cadastro em massa de referências e peças através de planilhas Excel.
* **Histórico Inteligente:** Registro rastreável de todas as entradas e produções com opção de exclusão seletiva.
* **Sincronização na Nuvem:** Integração nativa com **Supabase** para persistência de dados em tempo real.

---

## 💻 Tecnologias Utilizadas

* **Frontend:** HTML5, CSS3 (Responsivo) e JavaScript (Vanilla).
* **Backend/Banco de Dados:** [Supabase](https://supabase.com/) (PostgreSQL + Realtime).
* **Iconografia:** Emojis e design focado em UX Industrial.

---

## 🚀 Como Utilizar

1.  **Cadastro:** Inicie cadastrando suas Referências e, em seguida, as Peças vinculadas a elas.
2.  **Estrutura (BOM):** Na aba BOM, defina a "receita" de cada produto (quantas peças cada unidade consome).
3.  **Movimentação:**
    * Use a aba **Entrada** para abastecer o estoque de peças.
    * Use a aba **Produção** para fabricar produtos (o sistema abaterá automaticamente os componentes do estoque).
4.  **Exportação:** Gere inventários específicos para conferência física através do botão "CSV" na aba de Estoque.

---

## ⌨️ Atalhos de Teclado

* `Alt + 1`: Dashboard
* `Alt + 2`: Cadastro
* `Alt + 3`: BOM
* `Alt + 4`: Entrada
* `Enter`: Confirma cadastros e movimentações rapidamente.

---

## 📄 Licença
Este projeto é de uso interno para a gestão da Elka Plásticos.
