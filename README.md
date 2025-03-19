<p align="center">
<img src="src/lib/img/logo/smxlogo.png" alt="SMX Logo" width="25%">
</p>

<h1 align="center">SMX <br> SMRT MRKT X © OFFICIAL WEBSITE</h1>

<h5 align="center"> version 1.0.0 </h5>

### We create amazing open-source projects that empower developers and foster collaboration.

```bash
~$ deploy
```

#### Developing

```bash
git clone https://github.com/SmrtMrktX/SMX.git
npm install
npm run dev

# follow the localhost link
```

Everything inside `src/lib` is part of your library, everything inside `src/routes` can be used as a showcase or preview app.

#### Contribution

```bash
Fork repo - Create your own branch - Make the app better - Commit it - Pull request.
```

#### Building

To build your library:

```bash
npm run package
```

To create a production version of your showcase app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.

#### Publishing

Go into the `package.json` and give your package the desired name through the `"name"` option. Also consider adding a `"license"` field and point it to a `LICENSE` file which you can create from a template (one popular option is the [MIT license](https://opensource.org/license/mit/)).

To publish your library to [npm](https://www.npmjs.com):

```bash
npm publish
```
