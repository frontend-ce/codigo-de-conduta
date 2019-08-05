# Código de Conduta dos eventos

Participantes, palestrantes, representantes de empresas e pessoas voluntárias do evento precisam concordar com este código de conduta. A equipe organizadora vai reforçar que este código seja seguido durante todo o evento. Esperamos a cooperação de todas as partes para ajudar a garantir um ambiente seguro para qualquer pessoa.
## Precisa de ajuda?

Você tem nossos contatos nos emails previamente enviados.
## Versão rápida

Nossa conferência é dedicada a fornecer uma experiência livre de assédio para todas as pessoas, independentemente do sexo, identidade de gênero e expressão, idade, orientação sexual, deficiência, aparência física, tamanho corporal, cor de pele, etnia, religião (ou falta dela) ou escolhas de tecnologias. Não toleramos o assédio a participantes do evento, sob qualquer forma. Linguagem e imagens sexuais não são apropriadas em nenhum local, incluindo palestras, workshops, festas, Twitter e outras mídias on-line. Violações destas regras poderão causar expulsão do evento, sem restituição, a critério da equipe organizadora.
## Versão mais longa

Constituem assédio comentários verbais ofensivos, e qualquer tipo de materiais ofensivos relacionados a gênero, identidade de gênero e expressão, idade, orientação sexual, deficiência, aparência física, tamanho corporal, cor de pele, etnia, religião, escolhas de tecnologias, imagens sexuais em espaços públicos, intimidação deliberada, perseguição, stalking, fotografias ou filmagens constrangedoras, interrupção contínua das apresentações ou outros eventos, contato físico inadequado e atenção sexual indesejada.

Participantes que receberem uma solicitação para interromper qualquer comportamento de assédio devem fazer isso imediatamente.

As políticas antiassédio também se aplicam a representantes de empresas patrocinadoras. Em particular, não devem usar imagens, atividades ou outro material de cunho sexual. As equipes de estandes e tendas (incluindo pessoas voluntárias) não devem utilizar roupas, uniformes ou trajes sexualizados ou criar um ambiente sexualizado de quaisquer formas.

Se alguém se envolver em comportamento de assédio, a equipe organizadora poderá tomar todas as medidas que considerar adequadas, incluindo avisar a pessoa ofensora ou expulsá-la do evento sem nenhum reembolso.

Caso sofra assédio, perceba que alguém esteja sofrendo assédio ou tenha alguma dúvida, entre em contato com alguém da organização imediatamente. As pessoas da equipe do evento podem ser identificadas, pois estarão vestindo camisetas marcadas.

A organização estará disposta a auxiliar participantes a entrar em contato com a segurança do hotel ou local, bem como aplicar a legislação pertinente, fornecer escoltas ou ajudar pessoas que sofrerem assédio para que se sintam seguras durante a conferência. Valorizamos sua participação.

Esperamos que todas as pessoas participantes sigam estas regras em salas de apresentação e workshops do evento, além de eventos sociais relacionados.

> Crédito e fonte original: http://2012.jsconf.us/#/about & [The Ada Initiative](http://geekfeminism.wikia.com/wiki/Conference_anti-harassment/Policy)
> Por favor, ajude a traduzir ou a melhorar: http://github.com/leftlogic/confcodeofconduct.com
> Esta obra está licenciada sob [Creative Commons Attribution 3.0 Unported License](https://creativecommons.org/licenses/by/3.0/deed.en_US)

<!-- This project was bootstrapped with [Create Next App](https://github.com/segmentio/create-next-app).

Find the most recent version of this guide at [here](https://github.com/segmentio/create-next-app/blob/master/lib/templates/default/README.md). And check out [Next.js repo](https://github.com/zeit/next.js) for the most up-to-date info.

## Table of Contents

- [Questions? Feedback?](#questions-feedback)
- [Folder Structure](#folder-structure)
- [Available Scripts](#available-scripts)
  - [npm run dev](#npm-run-dev)
  - [npm run build](#npm-run-build)
  - [npm run start](#npm-run-start)
- [Using CSS](#using-css)
- [Adding Components](#adding-components)
- [Fetching Data](#fetching-data)
- [Custom Server](#custom-server)
- [Syntax Highlighting](#syntax-highlighting)
- [Using the `static` Folder](#using-the-static-folder)
- [Deploy to Now](#deploy-to-now)
- [Something Missing?](#something-missing)

## Questions? Feedback?

Check out [Next.js FAQ & docs](https://github.com/zeit/next.js#faq) or [let us know](https://github.com/segmentio/create-next-app/issues) your feedback.

## Folder Structure

After creating an app, it should look something like:

```
.
├── README.md
├── components
│   ├── head.js
│   └── nav.js
├── next.config.js
├── node_modules
│   ├── [...]
├── package.json
├── pages
│   └── index.js
├── static
│   └── favicon.ico
└── yarn.lock
```

Routing in Next.js is based on the file system, so `./pages/index.js` maps to the `/` route and
`./pages/about.js` would map to `/about`.

The `./static` directory maps to `/static` in the `next` server, so you can put all your
other static resources like images or compiled CSS in there.

Out of the box, we get:

- Automatic transpilation and bundling (with webpack and babel)
- Hot code reloading
- Server rendering and indexing of `./pages`
- Static file serving. `./static/` is mapped to `/static/`

Read more about [Next's Routing](https://github.com/zeit/next.js#routing)

## Available Scripts

In the project directory, you can run:

### `npm run dev`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any errors in the console.

### `npm run build`

Builds the app for production to the `.next` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

### `npm run start`

Starts the application in production mode.
The application should be compiled with \`next build\` first.

See the section in Next docs about [deployment](https://github.com/zeit/next.js/wiki/Deployment) for more information.

## Using CSS

[`styled-jsx`](https://github.com/zeit/styled-jsx) is bundled with next to provide support for isolated scoped CSS. The aim is to support "shadow CSS" resembling of Web Components, which unfortunately [do not support server-rendering and are JS-only](https://github.com/w3c/webcomponents/issues/71).

```jsx
export default () => (
  <div>
    Hello world
    <p>scoped!</p>
    <style jsx>{`
      p {
        color: blue;
      }
      div {
        background: red;
      }
      @media (max-width: 600px) {
        div {
          background: blue;
        }
      }
    `}</style>
  </div>
)
```

Read more about [Next's CSS features](https://github.com/zeit/next.js#css).

## Adding Components

We recommend keeping React components in `./components` and they should look like:

### `./components/simple.js`

```jsx
const Simple = () => <div>Simple Component</div>

export default Simple // don't forget to export default!
```

### `./components/complex.js`

```jsx
import { Component } from 'react'

class Complex extends Component {
  state = {
    text: 'World'
  }

  render() {
    const { text } = this.state
    return <div>Hello {text}</div>
  }
}

export default Complex // don't forget to export default!
```

## Fetching Data

You can fetch data in `pages` components using `getInitialProps` like this:

### `./pages/stars.js`

```jsx
const Page = props => <div>Next stars: {props.stars}</div>

Page.getInitialProps = async ({ req }) => {
  const res = await fetch('https://api.github.com/repos/zeit/next.js')
  const json = await res.json()
  const stars = json.stargazers_count
  return { stars }
}

export default Page
```

For the initial page load, `getInitialProps` will execute on the server only. `getInitialProps` will only be executed on the client when navigating to a different route via the `Link` component or using the routing APIs.

_Note: `getInitialProps` can **not** be used in children components. Only in `pages`._

Read more about [fetching data and the component lifecycle](https://github.com/zeit/next.js#fetching-data-and-component-lifecycle)

## Custom Server

Want to start a new app with a custom server? Run `create-next-app --example customer-server custom-app`

Typically you start your next server with `next start`. It's possible, however, to start a server 100% programmatically in order to customize routes, use route patterns, etc

This example makes `/a` resolve to `./pages/b`, and `/b` resolve to `./pages/a`:

```jsx
const { createServer } = require('http')
const { parse } = require('url')
const next = require('next')

const dev = process.env.NODE_ENV !== 'production'
const app = next({ dev })
const handle = app.getRequestHandler()

app.prepare().then(() => {
  createServer((req, res) => {
    // Be sure to pass `true` as the second argument to `url.parse`.
    // This tells it to parse the query portion of the URL.
    const parsedUrl = parse(req.url, true)
    const { pathname, query } = parsedUrl

    if (pathname === '/a') {
      app.render(req, res, '/b', query)
    } else if (pathname === '/b') {
      app.render(req, res, '/a', query)
    } else {
      handle(req, res, parsedUrl)
    }
  }).listen(3000, err => {
    if (err) throw err
    console.log('> Ready on http://localhost:3000')
  })
})
```

Then, change your `start` script to `NODE_ENV=production node server.js`.

Read more about [custom server and routing](https://github.com/zeit/next.js#custom-server-and-routing)

## Syntax Highlighting

To configure the syntax highlighting in your favorite text editor, head to the [relevant Babel documentation page](https://babeljs.io/docs/editors) and follow the instructions. Some of the most popular editors are covered.

## Deploy to Now

[now](https://zeit.co/now) offers a zero-configuration single-command deployment.

1.  Install the `now` command-line tool either via the recommended [desktop tool](https://zeit.co/download) or via node with `npm install -g now`.

2.  Run `now` from your project directory. You will see a **now.sh** URL in your output like this:

    ```
    > Ready! https://your-project-dirname-tpspyhtdtk.now.sh (copied to clipboard)
    ```

    Paste that URL into your browser when the build is complete, and you will see your deployed app.

You can find more details about [`now` here](https://zeit.co/now).

## Something Missing?

If you have ideas for how we could improve this readme or the project in general, [let us know](https://github.com/segmentio/create-next-app/issues) or [contribute some!](https://github.com/segmentio/create-next-app/edit/master/lib/templates/default/README.md) -->
