# Getting Up and Running

The following steps will help you set up 1) a Craft installation, with pre-made content and 2) a basic Gridsome project that we'll be working on together.

If you have any trouble with setup, please ask Jake, Andris, or one of the other workshop volunteers.

## Craft

### 1. Database

Create a database named `ontherocks`, then import the database export named `ontherocks.sql` in the root of this repo.

### 2. Install dependencies

Run `composer install` to install all of the necessary dependencies.

### 3. Configure your environment

1. Clone `.env.example` to and create `.env`
1. Run `./craft setup/security-key` to create a security key
1. Open your new `.env`, and make any necessary configurations (DB server/user/pass, etc.)

## Gridsome

For these steps you'll need to run the following commands within the "frontend" folder, not in the project root. If you're in the project root, you can run `cd frontend`.

### 1. Install dependencies

Run `yarn` or `npm install` to install all of the necessary dependencies.

### 2. Make sure everything's working

Run `yarn dev` or `npm run dev`. Assuming you don't hit any errors (fingers crossed), when everything's done running you should see two URLs in the console: one will be the development site we'll be building on, and the second is a GraphQL playground that is integrated with Gridsome.

**Note**: Do not run `gridsome develop` directly, as this project has some pre/post command hooks set up

## Information

### Craft Admin Credentials
- Username: `admin`
- Password: `happyBrad`
