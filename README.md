# Angular 16 — Estrutura de Pastas e Arquivos

[← Voltar](https://github.com/JosiTubaroski/FullStackAngular16_DotNet/blob/main/README.md)

Quando um projeto **Angular 16** é criado usando o Angular CLI (com o comando `ng new nome-do-projeto`), ele já gera uma estrutura completa de arquivos e pastas, pensada para escalabilidade e boas práticas. Este guia resume a estrutura inicial e para que serve cada parte.

## Estrutura de Pastas Geradas pelo Angular 16

```
meu-projeto/
├── node_modules/
├── src/
│   ├── app/
│   │   ├── app.component.ts
│   │   ├── app.component.html
│   │   ├── app.component.css
│   │   └── app.module.ts
│   ├── assets/
│   ├── environments/
│   ├── index.html
│   ├── main.ts
│   └── styles.css
├── angular.json
├── package.json
├── tsconfig.json
└── README.md
```

## Entendendo Cada Parte

### `node_modules/`

- Pasta onde ficam todas as **dependências** do projeto (bibliotecas do Angular, entre outras).
- Criada automaticamente ao rodar `npm install`.

### `src/`

Onde vive o **código-fonte** da aplicação — componentes, módulos, serviços e rotas.

- `app.component.ts` — lógica do componente principal (`AppComponent`).
- `app.component.html` — HTML do `AppComponent`.
- `app.component.css` — estilo do `AppComponent`.
- `app.module.ts` — **módulo raiz**, onde os componentes são declarados e outros módulos são importados.

### `src/assets/`

- Onde ficam imagens, fontes e outros arquivos estáticos usados no front-end.

### `src/environments/`

- Define as variáveis de ambiente da aplicação:
  - `environment.ts` — ambiente de **desenvolvimento**.
  - `environment.prod.ts` — ambiente de **produção**.

### `src/index.html`

- HTML base da aplicação — é aqui que o Angular injeta o app.

### `src/main.ts`

- **Ponto de entrada** da aplicação Angular.
- Carrega o `AppModule` e inicializa o Angular.

### `src/styles.css` (ou `styles.scss`)

- Estilo global da aplicação.

## Arquivos de Configuração na Raiz do Projeto

| Arquivo | Descrição |
|---|---|
| `angular.json` | Arquivo de configuração do projeto Angular — define build, estilos, assets, scripts e outras configurações da CLI. |
| `package.json` | Lista as dependências do projeto (bibliotecas do Angular e de terceiros) e os scripts disponíveis (como `ng serve`, `ng build`). |
| `tsconfig.json` | Configurações do compilador TypeScript, usadas em todo o projeto. |
| `README.md` | Documentação padrão gerada automaticamente pelo Angular CLI ao criar o projeto. |
