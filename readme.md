Demoing an issue with {{yield}} in Svelte 1.3.0

```sh
npm install
npm test
```

Try these variations by changing `main.svelte`:

1. uncomment the commented block - it's still incorrect, but `person` is no longer undefined inside of the loop
2. move the commented block to after the loop - now it's undefined in each place, including outside of the loop
