# Poodle Shop

It stuck and paused.

## motivate

In order to learn nodejs in a fashion style I decided to create a bunch of serverless function in nodejs and deploy them to the aws lambda.

When lambda functions get more and more it becomes trivial. `monorepo` instantly comes up in my mind. Why not give it a try.

At very first I tried `nx`. However there is no plugin for aws lambda. The built-in node plugin is too big for lambda.

Then I think maybe the `npm workspace` is good enough. Everything is fine until the deployment.

When it comes to workspace the dependencies will be installed at root folder. However the lambda deployment requires `node_modules` involvement.

Emmm... After checking out the dev docs. There is no easy way to work around this. So Let's press `pause` button for now.

## requirement

npm version >= 7 (in order to )

## commands

- deploy

  - `npm run deploy`

- deploy single lambda
  - `npm run deploy:func -w [service name]`
