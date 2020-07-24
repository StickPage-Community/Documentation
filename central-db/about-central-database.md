# About Central Database

The Central Database is a collection of JSON files manually crafted by humans for the `@stickpage-api/json-db` Node.js package. The database is hosted on GitLab, and currently under work-in-progress for now.

## Getting Started

To access the database locally, clone it using Git.

```bash
## Directly from GitLab
git clone https://gitlab.com/StickPage/Database-Repository.git

## Or, use the GitHub mirror.
git clone https://github.com/StickPage-API/Central-DB.git
```

If you cloned the source files of `@stickpage-api/json-db` package, navigate to there and simply run the following these commands below.

```bash
## Run this command one and it will clone everything for you.
npm run db:clone

## Then choose what branch you want to work on
npm run db:list-remotes && npm run db:list-branches
npm run db:change-branch origin master ## For development
## or use this for stable releases, arguments in 'git checkout' allowed.
npm run db-change-branch origin pr-wip/json-schema-validator.
```

See the following links to learn more on how to contribute to the database.

{% page-ref page="schema/" %}

{% page-ref page="add-entry.md" %}



