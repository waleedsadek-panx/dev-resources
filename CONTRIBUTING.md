# Contributing

Everyone is encouraged to collaborate and add new resources to the list, but please take into consideration the following:

-   the resource should align with the purpose of the project
-   the resource isn't a duplicate; a text search on the README file should be enough to find this answer

## Adding a resource

-   resources are organized alphabetically in separate files in the `resources` folder; use the resource `name` property to determine which file it belongs to
-   within the file, keep the alphabetical order, again based on the resource `name` property

### Resource format

Each resource belongs to an object, as such:

```javascript
{
    name: 'freeCodeCamp',
    description:
        'Learn to code at home. Build projects. Earn certifications. Since 2014, more than 40,000 freeCodeCamp.org graduates have gotten jobs at tech companies including Google, Apple, Amazon, and Microsoft.',
    icon: 'https://www.freecodecamp.org/news/favicon.png',
    categories: [programming.learn, programming.codeChallenges],
    links: {
        [website]: 'https://www.freecodecamp.org',
        [youtube]: 'https://www.youtube.com/c/freecodecamp',
    },
},
```

Observe that:

-   `categories` is an array, meaning the resource can belong to multiple categories
-   `links` is an object, where multiple platforms can be added
-   `categories` values (e.g. `programming.learn`) and `links` key properties (e.g. `[youtube]`) should be used from the `constants/categories.js` and `constants/links.js` files respectively; due to the dynamic nature of these values, they can receive updates and additions, so this ensures organization and avoids misspellings
-   `icon` is the only optional property, all others are required, with `categories` and `links` containing at least one value
-   the `description` property can be custom or grabbed from the resource's metadata included in the `<head>` tag of the website's HTML document
-   the `icon` property can also be grabbed from the resource's metadata included in the `<head>` tag or by doing the following:

    1. navigate to https://favicongrabber.com
    2. insert the resource's URL
    3. open the result image in a new tab by right clicking followed by "Open in new tab" or dragging it to the browser's tab bar
    4. use the new tab's URL

## Code formatting and linting

This project relies on [Prettier](https://prettier.io/) and [ESLint](https://eslint.org/) for code formatting and error/standards checking, so please ensure you have both installed globally or run `npm install` in order to install them in the project directory.

## Need assistance?

The resources list is created in JavaScript, and if you're unable to make a contribution for this or any other reason, feel free to open an issue explaininig your situation, so another developer can help you getting your resource in the lists.

---

## Thank you for contributing