# Hasura GraphQL Engine on Heroku

This backend is powered by the Hasura GraphQL Engine, which is a blazing-fast GraphQL server that gives you :zap: **instant,
realtime GraphQL APIs over Postgres**, with [**webhook
triggers**](https://github.com/hasura/graphql-engine/blob/master/event-triggers.md)
on database events for asynchronous business logic.

We deploy Hasura GraphQL Engine on Heroku and get a GraphQL endpoint for use in our Gatsby app.

## Useful commands

Copy databases between apps:

```
heroku pg:copy recipe-palette::DATABASE_URL DATABASE_URL --app recipe-palette-dev
```

Set a remote to the Heroku Git url:

```
git remote add heroku <heroku-git-url>
```

Push an empty commit to Heroku to trigger a build (with automatic deploys enabled):

```
git commit --allow-empty "trigger build" && git push heroku master
```

## Further reading

- [Building your schema](https://docs.hasura.io/1.0/graphql/manual/schema/index.html)
- [GraphQL Queries](https://docs.hasura.io/1.0/graphql/manual/queries/index.html)
- [GraphQL Mutations](https://docs.hasura.io/1.0/graphql/manual/mutations/index.html)
- [GraphQL Subscriptions](https://docs.hasura.io/1.0/graphql/manual/subscriptions/index.html)
- [Event Triggers](https://docs.hasura.io/1.0/graphql/manual/event-triggers/index.html)
- [Authentication/Access control](https://docs.hasura.io/1.0/graphql/manual/auth/index.html)
- [Database Migrations](https://docs.hasura.io/1.0/graphql/manual/migrations/index.html)
- [Guides/Tutorials/Resources](https://docs.hasura.io/1.0/graphql/manual/guides/index.html)
