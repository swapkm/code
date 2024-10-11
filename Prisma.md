## Prisma Initialization

`npx prisma init`

Initializes Prisma in your project by setting up a prisma folder containing schema.prisma, and the configuration for your database.

## Generate Prisma Client

`npx prisma generate`

Generates the Prisma Client based on your schema.prisma. After modifying your schema, you must run this command to update the client.

## Database Migration

`npx prisma migrate dev --name init`

Creates a new migration file based on changes to your schema and applies the migration to your development database.

## Migrate deploy

`npx prisma migrate deploy`

Applies pending migrations to your production database.

## Status

`npx prisma migrate status`

Shows the status of your migrations, indicating which ones have been applied and which are pending.

## Push the current schema directly to the database

`npx prisma db push`

Pushes your schema.prisma changes to your database without creating a migration. Use this in development environments.

## Re-introspect the schema from the database using:

`npx prisma db pull`

This will update your schema.prisma based on the existing database schema

## Prisma Studio

`npx prisma studio`

Launches an interactive database GUI to visualize and edit your database records.

## Format Prisma Schema

`npx prisma format`

Automatically formats your schema.prisma file according to Prisma's formatting rules.

## Reset

`npx prisma migrate reset`

Drops all tables in the database (complete data loss).
Looks for migration files in the prisma/migrations/ folder if found apply that schema, if not found remain empty.
