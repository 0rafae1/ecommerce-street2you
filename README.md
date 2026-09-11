# Street2You 👟🔥

> *As ruas que encontram você.*

A **Street2You** é uma landing page moderna e responsiva de e-commerce voltada para a moda urbana e cultura streetwear. O projeto foi desenvolvido com foco em boas práticas de estruturação semântica, organização modular de estilos e design responsivo adaptado para diferentes tamanhos de tela.

---

## 📌 Sumário

- [Visão Geral](#-visão-geral)
- [Funcionalidades e Seções](#-funcionalidades-e-seções)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Destaques Técnicos](#-destaques-técnicos)
- [Próximos Passos](#-próximos-passos)
- [Autor](#-autor)

---

## 🎯 Visão Geral

O projeto apresenta a vitrine digital da marca **Street2You**, trazendo coleções de calçados e vestuário como Techwear, Básico, Urbano e Esportivo. 

A interface combina estética visual limpa com navegação intuitiva, oferecendo ao usuário uma experiência imersiva inspirada nos maiores e-commerces de moda urbana do mundo.

---

## ✨ Funcionalidades e Seções

- **Header Flutuante e Navegação:**
  - Barra de navegação com cantos arredondados flutuando no topo da página.
  - Links para categorias principais (*Masculino*, *Feminino*, *Outlet*).
  - Ícones de ação rápida para perfil de usuário, central de ajuda e sacola de compras.
  - **Menu Hambúrguer 100% CSS** para dispositivos móveis, sem necessidade de JavaScript (técnica do *checkbox hack*).

- **Seção Hero (Destaque Principal):**
  - Banner com imagem em alta resolução e tipografia marcante com sombra (*text-shadow*).
  - Chamada para ação (CTA) com botões *"Comprar"* e *"Mais modelos"*.
  - Imagem de fundo responsiva dedicada para telas menores (*mobile*).

- **Categorias em Destaque:**
  - Cards visuais com efeito de sobreposição escura (*overlay*) para destacar as categorias: **Básico**, **Urbano**, **Esportivo** e **Techwear**.

- **Grid de Produtos (Mosaico Assimétrico):**
  - Vitrine estilizada utilizando **CSS Grid** com áreas nomeadas (`grid-template-areas`).
  - Destaque especial para o produto **Black Lynx** com chamada para ver detalhes.
  - Reorganização automática e fluida para telas de tablets e celulares.

- **Rodapé Completo (Footer):**
  - Formulário para inscrição em newsletter.
  - Links de redes sociais (*Instagram*, *WhatsApp*, *YouTube* e *X*) estilizados com máscaras SVG dinâmicas.
  - Mapa de links do site com seções categorizadas.
  - Informações de direitos autorais (*Copyright*).

---

## 🛠 Tecnologias Utilizadas

- **HTML5 Semântico:** Uso correto de tags como `<header>`, `<nav>`, `<main>`, `<section>`, `<article>` e `<footer>` para melhor acessibilidade e SEO.
- **CSS3 Moderno:**
  - **CSS Grid Layout:** Criação do mosaico assimétrico de produtos.
  - **CSS Flexbox:** Alinhamentos e distribuição dos elementos do cabeçalho, categorias e rodapé.
  - **CSS Variables (Custom Properties):** Centralização de variáveis para paleta de cores e tipografia.
  - **Media Queries:** Adaptação responsiva para telas com larguras de 1280px, 1000px, 768px e 500px.
  - **Modern CSS Reset:** Reset global baseado na solução de *Andy Bell* para garantir consistência entre navegadores.
  - **SVG Masks (`mask-image`):** Uso de máscaras para controlar a cor e os efeitos de *hover* em ícones sem carregar múltiplos arquivos de imagem.
- **Tipografia:** Google Fonts ([Ubuntu](https://fonts.google.com/specimen/Ubuntu) e [Outfit](https://fonts.google.com/specimen/Outfit)).

---

## 💡 Destaques Técnicos

1. **Menu Hambúrguer sem JavaScript:**
   O menu responsivo mobile foi implementado combinando `<input type="checkbox">`, `<label>` e o seletor CSS `:checked ~ .nav-container`, demonstrando como recursos avançados de CSS podem resolver interações de interface de forma leve e performática.

2. **Arquitetura CSS Modular:**
   Ao invés de um único arquivo de estilos gigantesco, os estilos foram divididos em pequenos arquivos na pasta `css/components/`, cada um focado em uma única responsabilidade.

3. **Coloração Dinâmica de Ícones SVG:**
   Com a propriedade `-webkit-mask-image` / `mask-image`, os ícones SVG utilizam uma única fonte de arquivo e têm sua cor alterada através da propriedade `background-color`, inclusive nos estados de `:hover`.

---

## 🔮 Próximos Passos

- [ ] Implementar interatividade com JavaScript (carrinho de compras, cálculo de frete, busca).
- [ ] Validação do formulário de newsletter.
- [ ] Adicionar modal de detalhes do produto ao clicar em *"detalhes"*.
- [ ] Implementar tema escuro (*dark mode*).

---

## 👨‍💻 Autor

Desenvolvido por **Rafael** durante os estudos no curso **Dev Quest**.