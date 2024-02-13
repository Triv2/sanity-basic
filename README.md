# Sanity-Basic
> A simple small project to get familiar with Sanity CMS and all it's features.

## Introduction

This project is an exploration of next.js and Sanity CMS combined. It is meant to be used as a learning tool for implementing
Sanity, using it for CRUD operations and back-end content management.

## Setup

Setup an account at https://www.sanity.io/ 

Start a new project on the dashboard, and for your first project copy the CLI they provide.

It will connect your local environment to your dashboard.

If it is your 2nd project follow the setup below:

### CLI Setup

- Create Next.js typescript application

```npx create-next-app@latest sanity-basic --typescript --tailwind --eslint```

<img src="https://github.com/Triv2/sanity-basic/assets/126743500/d5430e5e-2232-4070-a9da-f8dc9d89495c" alt="next-setup" width={500} height={200} />


- Create Sanity Project and connect to your Sanity dashboard

```npm -y create sanity@latest```

<img src="https://github.com/Triv2/sanity-basic/assets/126743500/b4b0549f-29a1-42bd-aa8f-70639381a24b" alt="next-setup" width={400} height={700} />

- Not sure if this is something wrong on my end, or what. Will update this section if I figure it out. But need to add quotes to the tsconfig.json target.

<img src="https://github.com/Triv2/sanity-basic/assets/126743500/e29c683f-d769-4b48-a93e-2fe5d840ce29" alt="next-setup" width={300} height={500} />


## How It Works

On the backend sanity schamas are setup, similar to react form schemas. These schemas are automatically added to the database and the content management system once built.
To access the data on the front-end Sanity uses GROQ queries. These are simple strings attached to a fetch query that selective read the values in the string. 
