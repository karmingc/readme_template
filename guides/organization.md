# Directory Structure

> Guidance - provide as much explanation as is helpful in understanding how to navigate and contribute to your repository. If your repo uses a framework like `Next.js` that has some structure out of the box, it would be helpful to link to any relevant documentation. [Laravel](https://laravel.com/docs/8.x/structure) has good documentation on the structure of a Laravel project that might provide a helpful example. 

The following guide is intended to help you navigate and contribute to our project. `src/App.tsx` is the entry point to our React application. Don't hesitate to ask questions if you don't know where to find or put something!

```
my-project/
    guides/
    src/
        atoms/
        hooks/
        navigation/
        pages/
        utils/
```

### Table of Contents
* [The Root Directory](#the-root-directory)
  * [The `guides` Directory](#the-guides-directory)
  * [The `src` Directory](#the-src-directory)
    * [The `atoms` Directory](#the-atoms-directory)
    * [The `hooks` Directory](#the-hooks-directory)
    * [The `navigation` Directory](#the-navigation-directory)
    * [The `pages` Directory](#the-pages-directory)
    * [The `utils` Directory](#the-utils-directory)
* [Additional Guidance](#additional-guidance)

### The Root Directory

#### The guides Directory
The `guides` directory is where you can find more thorough documentation that doesn't necessarily belong in the README.

### The src Directory

#### The atoms Directory
The `src/atoms` directory is where our lowest level React components live. These components are the building blocks that are used across many parts of our UI.

#### The hooks Directory
The `src/hooks` directory is where our custom-built React hooks live. This is one of the ways we share complex component logic across our app.

#### The navigation Directory
The `src/navigation` directory is where you can find the navigation routes and any navigator components.

#### The pages Directory
The `src/pages` directory is where our Page components live. These components are the entry point to a specific route. They're the opposite of `atoms`, in that they are the highest level components in our repo.

#### The utils Directory
The `src/utils` directory is where all of our utility classes and helper functions live.

### Additional Guidance

* We co-locate Tests and Storybooks with the components they reference.
* We group pages that are part of a specific flow or feature in a directory together.
* When deciding where to put a component, we provide the following guidance...
    * Components that are used widely across the UI belong in `src/atoms`
    * Components that are the entry point to a route belong in `src/pages`
    * Components that are only used for one screen or shared across one flow likely belong in the directory for the page or flow they are relevant too instead of `src/atoms`

Given that the organization for a Page component may look something like...

```
src/
    pages/
        PageA/
            HelperA/
                HelperA.tsx
                HelperA.test.tsx
                HelperA.stories.tsx
                index.ts
            HelperB/
                HelperB.tsx
                HelperB.test.tsx
                HelperB.stories.tsx
                index.ts
            PageA.tsx
            PageA.test.tsx
            index.ts
```

The organization of several pages that are part of the same feature or flow may look something like...

```
src/
    pages/
        feature-a/
            PageA/
            PageB/
            PageC/
```

Don't hesitate to ask questions if you are sure where to find something or put something!