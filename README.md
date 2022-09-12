# Poodle Shop

## motivate

In order to learn nodejs in a fashion style I decided to create a bunch of serverless function in nodejs and deploy them to the aws lambda.

However how to manage them becomes trivial. And monorepo comes up in my mind. Why not give it a try.

At very first I tried `nx`. However there is no plugin for aws lambda. The built-in node plugin is too big for lambda.

Then I think maybe the `npm workspace` is good enough.

## requirement

npm version >= 7 (in order to )

## commands

- deploy

  - `npm run deploy`

- deploy single lambda
  - `npm run deploy:func -w [service name]`
