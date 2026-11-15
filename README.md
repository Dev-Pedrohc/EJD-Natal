# EJD-Natal

Sistema de votação voltado para o encontro **EJD (Encontro Jovem Damas)**.

A ideia do projeto é ajudar o encontro de uma forma intuitiva, deixando-o mais interativo e com um site bonito, para que a galera possa se divertir. Para quem está desenvolvendo, o projeto também serve como aprendizado de front-end e banco de dados trabalhando juntos.

## 💚💙 Funcionalidades

- O sistema possui várias perguntas de votação, cada uma com **um número flexível de opções** (pode ser 4, 5, 6 ou mais).
- O sistema guarda cada voto em um banco de dados.
- O sistema define como vencedor quem receber **mais votos no dia** em cada pergunta.
- O sistema mostra um **ranking final** com, para cada pergunta, os vencedores e a contagem de votos.

## 🧱 Tecnologias

| Parte | Tecnologia |
|-------|-----------|
| Front-end | HTML, CSS e JavaScript |
| Banco de dados | MySQL |

## 🗄️ Banco de dados

O projeto usa **MySQL** para guardar as informações da votação:

- **Perguntas:** cada pergunta que será votada.
- **Opções:** as opções de cada pergunta (quantas forem necessárias).
- **Votos:** cada voto registrado, ligado a uma opção.

Com esses dados, o sistema consegue contar os votos e montar o ranking final com o vencedor de cada pergunta.

## 🗂️ Estrutura sugerida

```
votacao-ejd/
├── frontend/
│   ├── index.html        # tela de votação
│   ├── ranking.html      # tela do ranking final
│   ├── css/
│   │   └── style.css
│   └── js/
│       ├── votacao.js
│       └── ranking.js
└── README.md
```

## 🚀 Como rodar o projeto

### Pré-requisitos

- [Git](https://git-scm.com/)
- (Opcional) [VS Code](https://code.visualstudio.com/) com a extensão **Live Server**

### 1. Clonar o repositório

```bash
git clone <url-do-repositorio>
cd votacao-ejd
```

### 2. Abrir o front-end

Abra o arquivo `frontend/index.html` no navegador, ou clique com o botão direito nele no VS Code e escolha **Open with Live Server**.

## 👥 Equipe e organização

- 1 admin do repositório (organiza as tarefas e explica como cada parte funciona).
- 3 colaboradores, cada um trabalhando na sua própria **branch**.

Fluxo de trabalho:

1. Cada pessoa cria uma branch para a sua parte (ex.: `feature/frontend`, `feature/banco`, `feature/ranking`).
2. Faz commits pequenos e com mensagens claras.
3. Abre um Pull Request para a `main`.
4. O admin revisa e faz o merge.

## 🛣️ Próximos passos

- [ ] Implementar o bloqueio de voto repetido (guardar no navegador que a pessoa já votou naquela pergunta)
- [ ] Criar uma tela de administração para cadastrar perguntas e opções sem mexer no banco
- [ ] Deixar o site responsivo para votar pelo celular
- [ ] Atualizar o ranking em tempo real, sem recarregar a página
- [ ] Gerar um QR Code que leve direto para a tela de votação
- [ ] Publicar o site online (ex.: GitHub Pages) para a galera acessar
