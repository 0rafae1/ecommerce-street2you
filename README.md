# Street2You 👟🔥

> *As ruas que encontram você.*

A **Street2You** é uma landing page moderna e responsiva de e-commerce voltada para a moda urbana e cultura streetwear. O projeto foi desenvolvido com foco em boas práticas de estruturação semântica em HTML5, organização modular de estilos em CSS3 e design responsivo adaptado para múltiplos tamanhos de tela.

---

<div align="center">

[![Deploy com GitHub Pages](https://img.shields.io/badge/Acessar%20Projeto-GitHub%20Pages-2ea44f?style=for-the-badge&logo=github)](https://0rafae1.github.io/ecommerce-street2you/)

👉 **[Clique aqui para ver a demonstração online](https://0rafae1.github.io/ecommerce-street2you/)** 👈

</div>

---

## 📌 Sumário

- [Visão Geral](#-visão-geral)
- [Demonstração Online](#-demonstração-online)
- [Funcionalidades e Seções](#-funcionalidades-e-seções)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Destaques Técnicos](#-destaques-técnicos)
- [Como Visualizar o Projeto](#-como-visualizar-o-projeto)
- [Próximos Passos](#-próximos-passos)
- [Autor](#-autor)

---

## 🎯 Visão Geral

O projeto apresenta a vitrine digital da marca **Street2You**, trazendo coleções de calçados e vestuário como Techwear, Básico, Urbano e Esportivo. 

A interface combina estética visual limpa com navegação fluida, oferecendo ao usuário uma experiência imersiva inspirada nos principais e-commerces de moda urbana.

---

## 🌐 Demonstração Online

O site está publicado e pode ser acessado diretamente através do GitHub Pages:

🔗 **Link do Deploy:** [https://0rafae1.github.io/ecommerce-street2you/](https://0rafae1.github.io/ecommerce-street2you/)

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
  - **CSS Flexbox:** Alinhamento e distribuição dos elementos no cabeçalho, categorias e rodapé.
  - **CSS Variables (Custom Properties):** Centralização de variáveis para paleta de cores e tipografia.
  - **Media Queries:** Adaptação responsiva para telas com larguras de 1280px, 1000px, 768px e 500px.
  - **Modern CSS Reset:** Reset global baseado na solução de *Andy Bell* para garantir consistência entre diferentes navegadores.
  - **SVG Masks (`mask-image`):** Uso de máscaras para controlar a cor e os efeitos de *hover* em ícones sem a necessidade de múltiplos arquivos de imagem.
- **Tipografia:** Google Fonts ([Ubuntu](https://fonts.google.com/specimen/Ubuntu) e [Outfit](https://fonts.google.com/specimen/Outfit)).

---

## 📁 Estrutura do Projeto

O código foi organizado seguindo o conceito de arquitetura modular, facilitando a manutenção e a legibilidade:

```text
ecommerce-street2you/
│
├── assets/
│   └── images/
│       ├── banners/             # Banners de destaque (desktop e mobile)
│       ├── favicons/            # Ícones para navegadores, Android e iOS
│       ├── icons/               # Ícones vetoriais em formato SVG
│       └── products/            # Imagens dos produtos e categorias
│
├── css/
│   ├── base.css                 # Estilos globais e componentes reutilizáveis (botões)
│   ├── reset.css                # Reset de estilos para consistência entre navegadores
│   ├── variables.css            # Variáveis de cores e importação de fontes
│   └── components/              # Estilos isolados por componente/seção
│       ├── footer.css           # Estilização do rodapé e newsletter
│       ├── header.css           # Cabeçalho, navegação e menu mobile
│       ├── hero.css             # Banner de destaque inicial
│       ├── product-category.css # Cards das categorias de produtos
│       └── product-grid.css     # Grid assimétrico de produtos
│
├── js/                          # Diretório reservado para scripts futuros
├── index.html                   # Página principal da aplicação
└── README.md                    # Documentação do projeto
```

---

## 💡 Destaques Técnicos

1. **Menu Hambúrguer sem JavaScript:**
   O menu responsivo mobile foi implementado combinando `<input type="checkbox">`, `<label>` e o seletor CSS `:checked ~ .nav-container`, demonstrando como recursos avançados de CSS podem resolver interações de interface de forma leve e performática.

2. **Arquitetura CSS Modular:**
   Ao invés de um único arquivo de estilos extenso, os estilos foram divididos em pequenos arquivos na pasta `css/components/`, cada um focado em uma única responsabilidade.

3. **Coloração Dinâmica de Ícones SVG:**
   Com a propriedade `-webkit-mask-image` / `mask-image`, os ícones SVG utilizam uma única fonte de arquivo e têm sua cor alterada através da propriedade `background-color`, inclusive nos estados de `:hover`.

---

## 🚀 Como Visualizar o Projeto

### Opção 1: Visualizar Online (Sem instalar nada)
Você pode ver o projeto funcionando em produção diretamente pelo navegador:
👉 [https://0rafae1.github.io/ecommerce-street2you/](https://0rafae1.github.io/ecommerce-street2you/)

### Opção 2: Utilizando a extensão Live Server (VS Code)
1. Clone o repositório em sua máquina:
   ```bash
   git clone https://github.com/0rafae1/ecommerce-syntaxwear.git
   ```
2. Abra a pasta do projeto no **Visual Studio Code**.
3. Instale a extensão **Live Server** (caso ainda não tenha).
4. Clique com o botão direito no arquivo `index.html` e selecione **"Open with Live Server"**.
5. O projeto abrirá no seu navegador padrão com recarregamento automático a cada alteração salva.

### Opção 3: Abrir diretamente no navegador
1. Baixe ou clone o repositório.
2. Localize o arquivo `index.html` na pasta do projeto.
3. Dê dois cliques sobre ele para abrir em qualquer navegador de sua preferência.

---

## 🔮 Próximos Passos

- [ ] Implementar interatividade com JavaScript (carrinho de compras, cálculo de frete, barra de busca).
- [ ] Validação do formulário de newsletter.
- [ ] Adicionar modal de detalhes do produto ao clicar em *"detalhes"*.
- [ ] Implementar tema escuro (*dark mode*).

---

## 👨‍💻 Autor

Desenvolvido por **Rafael** durante os estudos no curso **Dev Quest**.