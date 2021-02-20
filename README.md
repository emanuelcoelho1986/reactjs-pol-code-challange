# React Polarising Code Exercise

> ...Front end is the hardest kind of dev I do. The folks who do it every day are heroes.

Tweet from: [Yehuda Katz](https://twitter.com/wycats/status/930463710941872128?ref_src=twsrc%5Etfw%7Ctwcamp%5Etweetembed%7Ctwterm%5E930463710941872128%7Ctwgr%5E%7Ctwcon%5Es1_&ref_url=https%3A%2F%2Fblog.logrocket.com%2Fthe-increasing-nature-of-frontend-complexity-b73c784c09ae%2F)

[The increasing nature of frontend complexity](https://blog.logrocket.com/the-increasing-nature-of-frontend-complexity-b73c784c09ae/)

***

## Why the challenge

Nowadays, the Frontend development scene has become more than simple HTML pages with CSS and some Javascript. In general, when developing Enterprise applications, there is the need to plan, design and architect how the WebSite (WebAPP/PWA/MOBILE/etc) will be done.

***
## Objective

The objective is to check how you think when approaching a problem.

***
## Expectations

Reusable code and not a lot of time invest in this coding exercise. It should be a quick thing to do.

***
## The Challenge

We have a list of Items with the following structure:

```typescript
interface Item {
    id: number;
    name: string;
    link?: string;
    children?: Item[];
}
```

We don't know the end of the tree, it's out of our control. We just know that everything is an <ul>.
We expect something like the following: 

```html
<ul>
    <li>Element 1</li>
    <li>Element 2</li>
    <li>
        <span>Element 3</span>
        <ul>
            <li>Element 4</li>
            <li>Element 5</li>
            <li>Element 6</li>
            <li>
                <span>Element 7</span>
                <ul>
                    <li>Element 8</li>
                    <li>Element 9</li>
                    <li>Element 10</li>
                </ul>
            </li>
        </ul>
    </li>
    <li>
        <span>Element 11</span>
        <ul>
            <li>Element 12</li>
            <li>
                <span>Element 13</span>
                <ul>
                    <li>Element 14</li>
                </ul>
            </li>
        </ul>
    </li>
    <li>Element 15</li>
    <li>Element 16</li>
</ul>
```
The example above is just some guidance. It doesn't mean that is the solution or uses things from the `items.json` source file.

***
## Requirements

- You should use the following technologies
    - ReactJS
    - TypeScript
    - Request the file remotely. The file is available at: [https://emanuelcoelho1986.github.io/reactjs-pol-code-challange/items.json](https://emanuelcoelho1986.github.io/reactjs-pol-code-challange/items.json)
    - There is no need to apply styles. Raw HTML will suffice.
- Nice to have:
    - At least one Class Component and one functional component
- Optional
    - Akita Store
    - Observables Approach instead of Promises
    - RxJS
    - Sort Items by name on each node

The Request library is up to you. Any of the choices available (Axios, Fetch, etc) are good.

***
## Instructions

- Build something similar to the HTML in the example above
- Make it available on Github (or similar) for us to check
- Inform us when we can check the solution
