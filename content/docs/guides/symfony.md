---
title: Connect from Symfony with Doctrine to Neon
subtitle: Set up a Neon project in seconds and connect from Symfony with Doctrine
enableTableOfContents: true
redirectFrom:
  - /docs/quickstart/symfony
  - /docs/integrations/symfony
updatedOn: '2023-10-19T23:10:12.837Z'
---

Symfony is a free and open-source PHP web application framework. Symfony uses the Doctrine library for database access. Connecting to Neon from Symfony with Doctrine is the same as connecting to a standalone Postgres installation from Symfony with Doctrine. Only the connection details differ.

To connect to Neon from Symfony with Doctrine:

1. [Create a Neon Project](#create-a-neon-project)
2. [Configure the connection](#configure-the-connection)

## Create a Neon project

If you do not have one already, create a Neon project. Save your connection details including your password. They are required when defining connection settings.

1. Navigate to the [Projects](https://console.neon.tech/app/projects) page in the Neon Console.
2. Click **New Project**.
3. Specify your project settings and click **Create Project**.

## Configure the connection

In your `.env` file, set the `DATABASE_URL` to the Neon project connection string that you copied in the previous step.

```shell
DATABASE_URL="postgres://[user]:[password]@[neon_hostname]/[dbname]?charset=utf8&sslmode=requre"
```


You can find all of the connection details listed above in the **Connection Details** widget on the Neon **Dashboard**. For more information, see [Connect from any application](/docs/connect/connect-from-any-app).

## Need help?

Join the [Neon community forum](https://community.neon.tech/) to ask questions or see what others are doing with Neon. [Neon Pro Plan](/docs/introduction/pro-plan) users can open a support ticket from the console. For more detail, see [Getting Support](/docs/introduction/support).
