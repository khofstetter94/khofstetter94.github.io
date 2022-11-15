# Gatsby, next.js, and other JS Frameworks

## Gatsby and next.js Resources

[Learn Next.js](https://nextjs.org/learn/basics/create-nextjs-app)

[Gatsby Tutorial](https://www.gatsbyjs.org/tutorial/)

[Next.js Docs](https://nextjs.org/docs)

[Gatsby.js Docs](https://www.gatsbyjs.com/docs/)

- Teach us two things about Next.js.
  - Data fetching in Next.js allows you to render your content in different ways, depending on your application's use case. These include pre-rendering with Server-side Rendering or Static Generation, and updating or creating content at runtime with Incremental Static Regeneration.
    - If you export a function called getServerSideProps (Server-Side Rendering) from a page, Next.js will pre-render this page on each request using the data returned by getServerSideProps.
    - getServerSideProps only runs on server-side and never runs on the browser. If a page uses getServerSideProps, then:
      - When you request this page directly, getServerSideProps runs at request time, and this page will be pre-rendered with the returned props
      - When you request this page on client-side page transitions through next/link or next/router, Next.js sends an API request to the server, which runs getServerSideProps
    - getServerSideProps returns JSON which will be used to render the page. All this work will be handled automatically by Next.js, so you don’t need to do anything extra as long as you have getServerSideProps defined.

- Teach us two things about Gatsby.js.
  - Redirects are settings in the network layer that allow you to route traffic from one url path to another with little to no disruption.
    - For instance, while rebuilding your cooking blog, you might want to move all of your recipes from their old path of blog/recipes to a new path of recipes. To make sure that all the existing links to your recipes still work, you would need a way to redirect your users from blog/recipes/mouthwatering-lasagna to recipes/mouthwatering-lasagna. No one wants to lose access to such a, well, mouthwatering recipe.
      - In gatsby-node.js, export the createPages method and use the createRedirects action to generate any redirects that you want to add. Here’s an example showing the lasagna recipe above:

        ```js
        exports.createPages = async ({ graphql, actions }) => {
          const { createRedirect } = actions

          createRedirect({
            fromPath: `/blog/recipes/mouthwatering-lasagna`,
            toPath: `/recipes/mouthwatering-lasagna`,
          })
        }
        ```

      - In the example above, you’ve explicitly redirected one of your recipe urls, and after adding a few others, you realize that you won’t have time to get all the old urls. So you decide that any other url that uses your old path blog/recipes/* should just be redirected to the new /recipes path. Here’s how you’d handle that:

      ```js
      exports.createPages = async ({ graphql, actions }) => {
      const { createRedirect } = actions

      createRedirect({
        fromPath: `/blog/recipes/mouthwatering-lasagna`,
        toPath: `/recipes/mouthwatering-lasagna`,
      })

        // All your other redirects

      createRedirect({
        fromPath: `/blog/recipes/*`,
        toPath: `/recipes`,
        })
      }
      ```

[Return home](https://khofstetter94.github.io/reading-notes/)
