# Aplicação com React e GraphQL

- graphql-codegen
- urql
- next
- tailwind
- graphcms
- ts-node
- typescript

> Usando GraphQL Codegen + Typescript

<pre>
  <code>
      overwrite: true

    schema: "$schema_graphcms$"

    documents: "./src/graphql/**/*.graphql"

    generates:
      src/generated/graphql.tsx:
        plugins:
          - "typescript"
          - "typescript-operations"
          - "typescript-urql"
        config:
          withHooks: true

    hooks:
      afterAllFileWrite:
        - eslint --fix
  </code>
</pre>

## Modelo Aplicação para um Blog

> Aplicação com as mecânicas básicas de um Blog possuindo Home Page, Posts Page, Post Content

- GraphQL Codegen para gerar as funções de queries
