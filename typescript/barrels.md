# Barrels

With barrels, it is better to explain by giving examples. Let's say you have multiple pages that you are importing into your `App.tsx` like so:

```ts
import { HomePage } from '../pages/HomePage'

import { AboutMePage } from '../pages/AboutMePage'

import { BlogPage } from '../pages/BlogPage'
```

We can actually consolodate this into a one-liner import by using *barrels*!.

Let's start by creating an `index.ts` file within the `pages` directory and then exporting all the pages we need in this file.

```ts
export * from './HomePage'
export * from './AboutMePage'
export * from './BlogPage'
```

Now that we have this exported, we can now go back into our `App.tsx` file and import them all in one line:

```ts
// App.tsx

import { HomePage, AboutMePage, BlogPage } from '../pages'
```

And that's how to use Barrels in TypeScript(JavaScript) to clean up some of your code and make importing/exporting more convenient. 