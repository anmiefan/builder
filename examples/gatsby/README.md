<h1 align="center">
  Using Builder.io with Gatsby
</h1>

> A demo for integrating [Builder.io](https://www.builder.io) with Gatsby using our GraphQL API and our `@builder.io/gatsby` plugin

This demo demonstrates creating dynamic pages in Builder.io on new URLs and generating them with Gatsby, as well
as rendering specific parts of your site with Builder.io content via GraphQL queries (e.g. for pages, components, etc)

See:

- [src/components/CodeBlock.tsx](src/components/CodeBlock.tsx) for an example of using a custom react component in the Builder.io visiaul editor. See a more rich example of a whole design system of components [here](https://github.com/BuilderIO/builder/tree/master/examples/react-design-system)
- [src/pages/example.tsx](src/pages/example.tsx) for using GraphQL to query and render Builder.io components and pages manually in parts of your Gatsby site and content
- [@builder.io/gatsby](https://github.com/builderio/builder/tree/master/packages/gatsby) the plugin used in this example to generate pages dynamically.

## 🚀 Quick start

1.  **Sign up for Builder.io**
    Then replace the demo API key in builder-config.js with your public API key, which you can find in [builder.io/account/organization](https://builder.io/account/organization)

2.  **Clone this demo.**

    ```bash
    git clone git@github.com:BuilderIO/builder.git
    cd builder/examples/gatsby
    npm install
    npm run dev
    ```

3.  **Connect Builder.io to your localhost**
    Now that you have the development server running on localhost, point the Builder.io entry to it by assigning the preview URL to be `http://localhost:3000`

<img width="796" alt="Screen Shot 2020-02-18 at 9 48 51 AM" src="https://user-images.githubusercontent.com/5093430/74763082-f5457100-5233-11ea-870b-a1b17c7f99fe.png">

When you deploy this to a live or staging environment, you can change the preview URL for your model globally from [builder.io/models](https://builder.io/models) (see more about models [here](https://builder.io/c/docs/guides/getting-started-with-models) and preview urls [here](https://builder.io/c/docs/guides/preview-url))
