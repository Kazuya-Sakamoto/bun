# bun 
公式ドキュメント: https://bun.sh/

**Bun is a fast JavaScript all-in-one toolkit**

### setup

```console
$ curl https://bun.sh/install | bash

$ exec /bin/zsh
```


### Why is Bun Fast
``` 
The Bun runtime exhibits impressive speed due to several key factors:

Lightweight Design: Bun is designed to be lightweight, resulting in a smaller codebase and reduced resource requirements.
This optimized design allows Bun to deliver better performance in terms of both speed and memory usage compared to other runtimes.

Low-Level Implementation: The Bun runtime is built using Zig, a relatively new low-level programming language.
Zig's characteristics enable developers to write code with fine-grained control over memory management and execution,
contributing to the runtime's efficiency.

Performance Optimization: Instead of relying on the V8 engine, Bun utilizes the JavaScriptCore from WebKit,
which is widely recognized for its superior performance. By leveraging this core engine, Bun benefits from its optimized execution of JavaScript code,
resulting in improved runtime speed.

Integrated Functionality: Bun offers native tools and features that streamline the development process.
It includes a built-in bundler, replacing the need for external tools like Webpack, as well as a native transpiler that supports writing TypeScript code directly. Additionally,
Bun incorporates a test runner similar to Jest and automatically loads environment variables without requiring additional installations of packages like dotenv.
```

引用: https://refine.dev/blog/bun-js-vs-node/#why-is-bun-fast


## install
### bun

```console
$ bun install
```

```console
bun install v1.0.2 (37edd5a6)
 + @nuxt/devtools@0.8.4
 + nuxt@3.7.3
✔ Types generated in .nuxt

 731 packages installed [516.00ms]
```

### yarn
```console
$ yarn install
```

```console
[4/4] 🔨  Building fresh packages...
✨  Done in 9.80s.
```

### npm

```console
$ npm intall
```

```console
added 1390 packages, and audited 1391 packages in 8s
```


## build time

### bun

```console
$ time bun run build
```

```console
Σ Total size: 2.33 MB (558 kB gzip)
✔ You can preview this build using node .output/server/index.mjs             nitro 10:09:11 PM
bun run build  7.32s user 0.90s system 144% cpu 5.693 total
```

### yarn

```console
$ time yarn run build
```

```console
ℹ Ready to run nuxt generate
✨  Done in 12.24s.
yarn run build  21.44s user 2.49s system 189% cpu 12.617 total
```

### npm

```console
$ time npm run build
```

```console
Ready to run nuxt generate
npm run build  10.30s user 1.01s system 233% cpu 4.843 total
```

## start development

### bun

```console
$ bun dev
```

```console
Nuxt 3.7.3 with Nitro 2.6.3
  ➜ Local:    http://localhost:3000/
  ➜ Network:  use --host to expose

✔ Nuxt DevTools is enabled v0.8.4 (experimental)                                   10:18:27 PM
ℹ Vite client warmed up in 841ms                                                   10:18:29 PM
✔ Nitro built in 446 ms
```

### yarn

```console
$ yarn dev
```

```console
✔ Client
  Compiled successfully in 3.78s

ℹ Waiting for file changes
ℹ Memory usage: 145 MB (RSS: 345 MB)
ℹ Listening on: http://localhost:3000/
```

### npm

```console
$ npm run dev
```

```console
✔ Client Compiled successfully in 2.02s

ℹ Waiting for file changes
ℹ Memory usage: 219 MB (RSS: 319 MB)
ℹ Listening on: http://localhost:3000/
No issues found.
```

## hot reload

### bun

```console
✔ Vite server hmr 6 files in 69.96ms
ℹ hmr update /app.vue (x3)
```

### yarn

```console
✔ Client
  Compiled successfully in 340.21ms

No issues found.
```

### npm

```console
✔ Client
  Compiled successfully in 102.13ms

No issues found.
```
