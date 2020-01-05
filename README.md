<h1 align="center">
  <img alt="Gympoint" title="Gympoint" src=".github/logo.png" width="200px" />
</h1>

<h3 align="center">
  Desafio Final: Gympoint
</h3>

<blockquote align="center">“O tempo que leva para realizar seus sonhos vai passar de qualquer forma”!</blockquote>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/rodrigocichetto/gympoint?color=%2304D361" />

  <a href="https://cichetto.com.br">
    <img alt="Made by Cichetto" src="https://img.shields.io/badge/made%20by-Cichetto-%232193b0">
  </a>

  <img alt="License" src="https://img.shields.io/badge/license-MIT-%2304D361" />
</p>

<p align="center">
  <a href="#-sobre-o-desafio">Sobre o desafio</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-layout">Layout</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#runner-run">Run</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-licença">Licença</a>
</p>

## 🚀 Sobre o desafio

Durante o desafio construi o app mobile da aplicação Gympoint utilizando React Native, a versão web utilizando React e o backend utilizando Node.JS.

## 🎨 Layout

O layout do desafio está em anexo([frontend](https://github.com/rodrigocichetto/bootcamp-gostack-desafio-09/blob/master/Gympoint.sketch), [mobile](https://github.com/rodrigocichetto/bootcamp-gostack-desafio-10/blob/master/Gympoint.sketch)) como um arquivo `.sketch`.

Caso esteja usando OS X / Windows você pode abrir esse arquivo com um software chamado [Zeplin](https://zeplin.io).

## :runner: Run

### Run backend

Acesse a pasta `backend`.

Instale as dependências

```bash
# using yarn
yarn
# or using npm
npm install
```

Configure suas váriaveis de ambiente `.env` a partir do arquivo [.env.example](https://github.com/rodrigocichetto/bootcamp-gostack-desafio-03/blob/master/.env.example). Obs.: As configurações de Database, Mongo e Redis do `.env.example` já estão setadas para os containers do `docker`

Inicie os containers a partir do [docker-compose.yml](https://github.com/rodrigocichetto/bootcamp-gostack-desafio-03/blob/master/docker-compose.yml) executando o comando `docker-compose up -d`

Execute as `migrations` e `seeds` do Sequelize

#### Sequelize Migrate
```bash
# using yarn
yarn sequelize db:migrate
# or using npm
npx sequelize db:migrate
```

#### Sequelize Seed
```bash
# using yarn
yarn sequelize db:seed:all
# or using npm
npx sequelize db:seed:all
```

Inicie o projeto

```bash
# using yarn
yarn dev:debug
# or using npm
npm run dev:debug
```

### Run frontend

Acesse a pasta `frontend`.

Instale as dependências

```bash
# using yarn
yarn
# or using npm
npm install
```

Inicie o projeto

```bash
# using yarn
yarn start
# or using npm
npm run start
```

### Run mobile

Acesse a pasta `mobile`.

Instale as dependências

```bash
# android && iOS
# using yarn
yarn
# or using npm
npm install

# iOS
cd ios/
pod install
```

Inicie o projeto. Obs.: O projeto mobile foi interamente desenvolvido no **iOS**.

```bash
# iOS
# using yarn
yarn ios
# or using npm
npm run ios

# android
# using yarn
yarn android
# or using npm
npm run android
```

## 📝 Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
