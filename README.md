# 🛒 Sacolão Digital

Um aplicativo web de página única (SPA) leve, rápido e responsivo desenvolvido para pequenos hortifrútis, sacolões e feirantes. O sistema permite que os clientes montem seus pedidos de forma intuitiva e os enviem diretamente para o WhatsApp do vendedor. Também conta com um painel administrativo simples para atualização de preços em tempo real.

## ✨ Funcionalidades

* **Catálogo de Produtos:** Exibição de produtos separados por categorias (Frutas, Legumes, Verduras) com imagens e preços por unidade/peso.
* **Carrinho de Compras Dinâmico:** Atualização em tempo real da quantidade de itens e valor total do pedido.
* **Checkout via WhatsApp:** O pedido é formatado automaticamente em uma mensagem clara e enviado diretamente para o WhatsApp do lojista.
* **Painel Administrativo Integrado:** Uma área restrita por senha onde o lojista pode editar os preços dos produtos.
* **Persistência de Dados:** As alterações de preços feitas no painel admin são salvas no cache do navegador (`localStorage`), mantendo os valores atualizados mesmo após recarregar a página.
* **Design Responsivo:** Interface otimizada para funcionar perfeitamente em celulares, tablets e computadores.

## 🛠️ Tecnologias Utilizadas

Este projeto não requer instalação de pacotes (Node.js, npm, etc). Ele roda inteiramente no navegador utilizando CDNs:

* **HTML5 / CSS3 / JavaScript**
* **[Vue.js 3](https://vuejs.org/)** (via CDN) - Para reatividade, controle de estado do carrinho e renderização dinâmica.
* **[Tailwind CSS](https://tailwindcss.com/)** (via CDN) - Para a estilização rápida e responsiva.
* **[FontAwesome](https://fontawesome.com/)** (via CDN) - Para os ícones da interface.

## 🚀 Como Executar o Projeto

Como o projeto é construído apenas com arquivos estáticos e CDNs, rodar o aplicativo é extremamente simples:

1.  Baixe o código-fonte (ou crie um arquivo `index.html` com o código fornecido).
2.  Dê um duplo clique no arquivo `index.html` para abri-lo em qualquer navegador web moderno (Chrome, Edge, Firefox, Safari).
3.  O aplicativo já estará funcionando!

## ⚙️ Configuração Importante (Lojista)

Para que os pedidos cheguem no WhatsApp correto, você **precisa alterar o número de telefone** no código-fonte.

1.  Abra o arquivo `index.html` em um editor de texto ou de código (como Bloco de Notas, VS Code, etc).
2.  Role até a linha `112` (ou busque por `const celular =`).
3.  Substitua o número fictício pelo número do seu negócio, incluindo o código do país (55 para o Brasil) e o DDD, sem espaços ou traços. Exemplo:
    ```javascript
    const celular = "5511988887777"; // Exemplo para o DDD 11
    ```

## 🔒 Acesso ao Painel Administrativo

Para alterar os preços dos produtos:

1.  Clique no botão **"Acesso Admin"** no cabeçalho (canto superior direito).
2.  Insira a senha padrão do administrador: **`BrunoGalvao`**
3.  Edite os preços diretamente nos campos amarelos que aparecerão nos produtos. As alterações são salvas automaticamente.
4.  Para voltar à visão de cliente, clique no botão **"Sair do Painel"**.

*(Dica: Para alterar a senha, busque por `BrunoGalvao` no código javascript e substitua pela senha desejada).*

## 👨‍💻 Autor

Desenvolvido por **Bruno Galvão**.
