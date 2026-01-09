# ⚙️ Projeto 2 - Automação Frontend

![Status](https://img.shields.io/badge/Status-Finalizado-green)
![Grunt](https://img.shields.io/badge/Task_Runner-Grunt-orange?logo=grunt&logoColor=white)
![LESS](https://img.shields.io/badge/Style-LESS-1d365d?logo=less&logoColor=white)
![HTML5](https://img.shields.io/badge/Code-HTML5-E34F26?logo=html5&logoColor=white)

> Uma Landing Page que implementa um fluxo de trabalho automatizado (pipeline), transformando código de desenvolvimento em ativos de produção otimizados.

## 🎯 Motivação e Propósito

Este projeto foi desenvolvido para aplicar conceitos de **Automação de Tarefas** e **Pré-processamento**. O propósito principal é resolver problemas comuns em grandes projetos web, como a desorganização de arquivos CSS extensos e o carregamento lento devido a scripts não minificados.

Ele demonstra a capacidade de configurar um ambiente onde tarefas repetitivas (como compilar LESS para CSS e comprimir JavaScript) são executadas automaticamente, garantindo um código final limpo e performático.

## 🛠️ Tecnologias Utilizadas

A arquitetura do projeto foca na separação entre ambiente de desenvolvimento (`src`) e produção (`dist`/`dev`), utilizando:

* **[Grunt](https://gruntjs.com/):** Task Runner responsável pela orquestração das tarefas.
  * `grunt-contrib-less`: Compilação de estilos.
  * `grunt-contrib-watch`: Monitoramento de arquivos em tempo real.
  * `grunt-contrib-uglify`: Minificação de JavaScript.
* **[LESS](https://lesscss.org/):** Pré-processador CSS que permite uso de variáveis, mixins e aninhamento.
* **[HTML5](https://developer.mozilla.org/pt-BR/docs/Web/HTML):** Estruturação semântica da página.
* **[Node.js & NPM](https://nodejs.org/):** Gerenciamento de dependências e pacotes do ambiente.

## 📦 Instalação e Configuração

Como este projeto depende de um Task Runner, é necessário instalar as dependências antes de executá-lo.

### Pré-requisitos
* **Node.js** (LTS) instalado na máquina.
* **Git** instalado.

### Passo a Passo

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/DouglassenG/projeto_2.git](https://github.com/DouglassenG/projeto_2.git)
    ```

2.  **Acesse o diretório:**
    ```bash
    cd projeto_2
    ```

3.  **Instale as dependências:**
    O comando abaixo lerá o arquivo `package.json` e baixará os plugins do Grunt necessários.
    ```bash
    npm install
    ```

4.  **Execute a Automação:**
    Para compilar o projeto e gerar os arquivos finais:
    ```bash
    npm run build
    # ou, se tiver o grunt-cli global:
    grunt
    ```

## 💻 Uso e Exemplos

O fluxo de trabalho configurado no `Gruntfile.js` permite que você edite os arquivos na pasta `src` e veja as alterações processadas automaticamente.

### Estrutura de Pastas
```text
projeto_2/
├── src/              # Código Fonte (Onde você edita)
│   ├── styles/       # Arquivos .less
│   ├── scripts/      # Arquivos .js originais
│   └── index.html    # Markup
├── dev/ (ou dist)    # Código Compilado (Gerado pelo Grunt)
│   ├── styles/       # CSS final
│   └── scripts/      # JS minificado
├── Gruntfile.js      # Configuração das tarefas
└── package.json      # Lista de dependências
