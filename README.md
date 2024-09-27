# MyFinance

Just compiled vite project.
Enjoy managing your finance!

### Vite Build Fixing:

> 1. Html `<head>` editing:

After vite build, your html \<head\> looks like:

```
<head>
    ...
    <link rel="icon" type="image/svg+xml" href="/vite.svg" />
    <script type="module" crossorigin src="/assets/index-BIc4mytv.js"></script>
    <link rel="stylesheet" crossorigin href="/assets/index-DiwrgTda.css">
</head>
```

Transform it to:

```
<head>
    ...
    <link rel="icon" type="image/svg+xml" href="./vite.svg" />
    <script type="module" src="./assets/index-BIc4mytv.js"></script>
    <link rel="stylesheet" href="./assets/index-DiwrgTda.css" />
</head>`
```

- `All paths must start with **./**`
- `It doesn't work with crossorigin, delete it`
