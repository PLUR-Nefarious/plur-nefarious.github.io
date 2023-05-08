# ChatbotsBattle.me 
An website with nothing but an input box for you to participate Once clicked you will be able to decide solo or multiplayer. I hope you enjoy and please let me know if there are any issues! 

Chatbots competing against each other as well as the players in text-games that have been a blast! 

Realtime chatbot game using GraphQL Live Queries, Next.js and NextAuth.js.
![ChatbotsBattle]

## Tools used
- NextAuth.js
- Next.js
- Apollo Client
- Server-Sent Events
- GraphQL Live Queries
- GraphQL
- Tailwind CSS

## Local Development

1. `npm install`
2. Create a [GitHub OAuth App](https://docs.github.com/en/apps/oauth-apps/building-oauth-apps/creating-an-oauth-app) with your app details for development purposes. Make sure to set `Authorization callback URL` to `http://localhost:3000/api/auth/callback/github`
3. `cp .env.example .env` and add values for `GITHUB_CLIENT_ID` and `GITHUB_CLIENT_SECRET` from step 2.
4. [Generate a secret value](https://generate-secret.vercel.app) for `NEXTAUTH_SECRET` and add it to `.env`
5. `npm run dev`

## Deploy to Production

1. Fork and Push this repo to GitHub
2. Create a [Vercel](https://vercel.com/) account
3. Connect your forked repo to Vercel
4. Add environment variable `NEXTAUTH_SECRET` during project creation
5. Create a [GitHub OAuth App](https://docs.github.com/en/apps/oauth-apps/building-oauth-apps/creating-an-oauth-app) with your app details for production purposes. Make sure to set `Authorization callback URL` to `[YOUR_DESIRED_VERCEL_DOMAIN]/api/auth/callback/github`
6. Deploy to Vercel and add `.env` values (`NEXTAUTH_SECRET`, `GITHUB_CLIENT_ID`, `GITHUB_CLIENT_SECRET`)




## Big thanks to Jamie Barton, Vercel, and Grafbase
https://grafbase.com/guides/how-to-build-a-real-time-chat-app-with-nextjs-graphql-and-server-sent-events
