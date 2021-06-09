<h1 align="center">Project name</h1>

> Guidance - brevity is important to building a culture of reading the docs. The README should be as short as it possibly can be, while providing the reader with the ability to run the repo locally. Thorough documentation is great, but consider whether some pieces of info need to be in the README or are better suited for an advanced guide.

Here's a one or two line description that provides helpful context about this project and how it fits into the rest of the Sonder eco-system.

## Table of Contents

- [Setup](#setup)
- [Contributing](#contributing)
- [Deployment](#deployment)
- [Advanced Guides](#advanced-guides)

## Setup

If you're just cloning the app, the following sections will help you get setup. If you've already run the app before, then you can probably skip ahead to the section about [running locally](#running-locally).

### OS Dependencies

#### Required

* `homebrew` in order to install other OS level dependencies.
* `node` version 16 must be installed to run this project.
* `yarn` is the JavaScript package we use in this project.
  
#### Optional

* `n` or `nvm` can be helpful in order to be able to easily change node versions. 

### Environment Variables

We've provided a sample environment variable file that you will want to copy from `.env.sample` to `.env`. Ask a teammate to help you get this set up.

### Running Locally

> Guidance - focus this section on whatever is the happiest path for getting the project running locally. In many cases that is against a staging environment. Unless it's necessary to have here, save more detailed instructions for how to run against local instances of other services for the [advanced guides](#advanced-guides) section.

The easiest way to run our application is against the `preview` staging environment, which can be done with the following command.

```shell
yarn start preview
```

See the [Advanced Guides] for more information about other helpful development tools and how to run this against project non-staging services.

## Contributing

> Guidance - use this section to explain or link to more detailed explanations of the expectations for contributing to your repo. Let any newcomers know about important code style or best practices that you follow. For example, a link to a testing guide would be appropriate here.

The following guides will be helpful to anyone who wants to contribute to our app. Please read through the following links before opening your first PR.

* Read our [testing guide](./guides/testing.md) to understand how we write tests.
* See the [organization guide](./guides/organization.md) to learn your way around the structure of our repo.
* The [internationalization guide](./guides/internationalization.md) explains how we internationalize text string using `i18n-next`.

## Deployment

> Guidance - add a description of the deployment process or link to a release guide here. Be sure to include instructions for deploying to any important environments. For example, include sections for `preview` and `production` if they differ.

This section includes instructions to deploy on [staging](#staging) and [production](#production) environment.

### Staging

### Production

## Advanced Guides

Here are some additional guides that you may or may not find helpful as you work in this repo.

* Running against a local `flatbook`
* API documentation
* Storybooks
