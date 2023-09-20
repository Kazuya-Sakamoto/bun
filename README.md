# 検証

## build time を計測

### bun

```
$ time bun run build
```

```
Σ Total size: 2.33 MB (558 kB gzip)
✔ You can preview this build using node .output/server/index.mjs             nitro 10:09:11 PM
bun run build  7.32s user 0.90s system 144% cpu 5.693 total
```

### yarn

```
$ time yarn run build
```

```
ℹ Ready to run nuxt generate
✨  Done in 12.24s.
yarn run build  21.44s user 2.49s system 189% cpu 12.617 total
```

### npm

```
$ time npm run build
```

```
Ready to run nuxt generate
npm run build  10.30s user 1.01s system 233% cpu 4.843 total
```

## 起動

### yarn

```
$ yarn dev
```

```
✔ Client
  Compiled successfully in 3.78s

ℹ Waiting for file changes
ℹ Memory usage: 145 MB (RSS: 345 MB)
ℹ Listening on: http://localhost:3000/
```

### bun

```
$ bun dev
```

```
Nuxt 3.7.3 with Nitro 2.6.3
  ➜ Local:    http://localhost:3000/
  ➜ Network:  use --host to expose

✔ Nuxt DevTools is enabled v0.8.4 (experimental)                                   10:18:27 PM
ℹ Vite client warmed up in 841ms                                                   10:18:29 PM
✔ Nitro built in 446 ms
```

### npm

```
$ npm run dev
```

```
✔ Client Compiled successfully in 2.02s

ℹ Waiting for file changes
ℹ Memory usage: 219 MB (RSS: 319 MB)
ℹ Listening on: http://localhost:3000/
No issues found.
```

## hot リロード

### bun

```
✔ Vite server hmr 6 files in 69.96ms
ℹ hmr update /app.vue (x3)
```

### yarn

```
✔ Client
  Compiled successfully in 340.21ms

No issues found.
```

### npm

```
✔ Client
  Compiled successfully in 102.13ms

No issues found.
```
