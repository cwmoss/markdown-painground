# supported syntax

## inline links, custom protokoll

    look at [our news page](cms:news)!

also works with autolinks

    look at our news page: <cms:news>

## mentions

    hello <@anna berger>, maybe we need better styling

??? in some cases, pointed brackets can be omitted

    hello @anna, maybe we need better styling

## custom atomic blocks

    !youtube[https://youtu.be/srGWeULxJr0?si=MArsUkMEUWZpz3ET&t=147]

    !author[312]

    !author[id="312" big avatar=rounded]

## custom blocks

    [contactform]

        [form-header]
            Please fill out the form. We'll answer you within two days
        [/form-header]

        !field[checkbox label="i want to subscribe to your newsletter"]

        !am-i-human[]

        We will **never** publish your email address or give it to any third party.

    [/contactform]

# implementations

## php

https://parsedown.org/demo
attribute parser: https://github.com/taufik-nurrohman/parsedown-extra-plugin
https://github.com/taufik-nurrohman/markdown

- must be able to render md to html

## js

- must be able to render md to html
- must be able to parse to ast
- must integrate to tiptap
- must integrate to easymde

https://marked.js.org/

## rust

- must be able to render md to html
- nice: convert md to ast
- nice: convert ast to md

# links

https://marked.js.org/
https://spec.commonmark.org/dingus/
https://tiptap.dev/docs/editor/markdown/api/utilities
