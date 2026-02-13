# SvelteKit Error reproduction repository

Run with 

```
pnpm install
pnpm dev
```

At the top you see Home / Route 1 / Route 2 and you can click around to see that navigation works.

The two buttons throw an in-page error. This error is not caught at all, but you can see it in the console. Afterwards, navigation keeps working.

The two "bad links" both also show an error in the console (+error doesn't get rendered), but after that, the navigation is broken. Clicking between home / route 1 / route 2 changes the URL in the URL bar but it doesn't actually change the rendered page.

Only the "non existent route" link always shows +error.
