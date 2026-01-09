---

### 🔗 Link 2: `projeto_2`

Este repositório marca a transição do "amador" para o "profissional". Aqui entra a **Build Tool** (Grunt ou Gulp) e o **CSS Pré-processado**. A documentação deve vender a ideia de que você sabe configurar um ambiente de desenvolvimento e não apenas escrever código solto.

#### 1. Descrição do Repositório (About)
*Copie e cole na seção "About" (lado direito) do seu repositório no GitHub.*

> **Descrição:** Landing Page com ambiente de desenvolvimento automatizado. Utiliza Grunt/Gulp para compilação de SASS, minificação de scripts e otimização de imagens, focando em performance e organização de código.

**Topics:** `grunt` `sass` `less` `automation` `frontend` `responsive-design` `web-performance`

#### 2. Arquivo README.md
*Copie o código abaixo para o arquivo `README.md`.*

```markdown
# ⚙️ Projeto 2 - Automação Frontend

![Status](https://img.shields.io/badge/Status-Finalizado-green)
![Grunt](https://img.shields.io/badge/Tool-Grunt%2FGulp-orange?logo=grunt)
![SASS](https://img.shields.io/badge/Style-SASS%2FLESS-pink?logo=sass)
![jQuery](https://img.shields.io/badge/Lib-jQuery-0769AD?logo=jquery)

> Uma aplicação web que implementa um fluxo de trabalho profissional, utilizando automação de tarefas para gerar um código final otimizado e performático.

## 🎯 Motivação e Propósito

O **Projeto 2** representa um salto técnico em relação ao desenvolvimento web estático. O objetivo principal aqui não foi apenas criar o layout, mas sim configurar um **Ambiente de Build**.

Este projeto resolve problemas comuns de desenvolvimento, como arquivos CSS gigantes e desorganizados (resolvido com SASS/LESS) e carregamento lento de página (resolvido com minificação automática de HTML, CSS e JS).

## 🖼️ Demonstração Visual

*(Insira aqui um print da Landing Page pronta)*

## 🛠️ Tecnologias Utilizadas

A stack foca na produtividade do desenvolvedor e performance do usuário final:

* **[SASS / LESS](https://sass-lang.com/):** Pré-processadores CSS para uso de variáveis, aninhamento (nesting) e mixins, tornando o estilo manutenível.
* **[Grunt / Gulp](https://gruntjs.com/):** Task Runner utilizado para vigiar arquivos (`watch`), compilar o SASS e comprimir o código para produção.
* **[jQuery](https://jquery.com/):** Biblioteca para manipulação simplificada do DOM e criação de interações (menus, máscaras de formulário).
* **[Node.js & NPM](https://nodejs.org/):** Gerenciamento das dependências de desenvolvimento.

## 📦 Instalação e Configuração

Diferente de sites estáticos simples, este projeto requer a instalação de dependências para compilar o código fonte.

### Pré-requisitos
* **Node.js** instalado na máquina.

### Passo a Passo

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/DouglassenG/projeto_2.git](https://github.com/DouglassenG/projeto_2.git)
    ```

2.  **Acesse a pasta:**
    ```bash
    cd projeto_2
    ```

3.  **Instale as dependências:**
    O comando abaixo lerá o arquivo `package.json` e instalará os plugins do Grunt/Gulp necessários.
    ```bash
    npm install
    ```

4.  **Execute o Build (Compilação):**
    Para gerar a pasta de distribuição (`dist`) e iniciar o modo de desenvolvimento:
    ```bash
    npm run build
    # ou simplesmente
    grunt
    ```

## 💻 Estrutura do Código

O projeto separa claramente o código de desenvolvimento (`src`) do código final (`dist` ou `build`):

```text
projeto_2/
├── src/              # Código Fonte (Editável)
│   ├── styles/       # Arquivos .scss ou .less
│   ├── scripts/      # Arquivos .js originais
│   └── index.html    # HTML original
├── dist/             # Código de Produção (Gerado automaticamente)
│   ├── css/          # CSS minificado
│   └── js/           # JS minificado/ofuscado
├── Gruntfile.js      # Configuração das tarefas de automação
├── package.json      # Lista de dependências
└── README.md         # Documentação
