# Open Source Wishlist

A list of open source projects I'd love made, but can't since I don't have as much time anymore.

## Imgix Clone

https://www.imgix.com

I love Imgix, but I don't love the pricing. 

1. There's a $10 monthly minimum
1. There's a per-master image cost, which makes it expensive for services that create a lot of one-time-use images like screenshots
1. The CDN pricing doesn't scale
1. Cache-busting is annoying

I would love a simple microservice that is API-compatible with Imgix that anyone can setup in their infrastructure and use their own CDN. Ideally, these built images would use Lambdas to resize them and would be saved to S3 for caching.

## Webhook Service

A library to easily create new webhooks that can be deployed as a server or as lambda functions. 

Some prior art:

- https://github.com/danistefanovic/hooka

Webhooks are a little annoying to implement because everyone implements them differently. I'd want the configuration options not to be about business logic but about validating the webhooks. Validations webhooks usually have are:

- IP address whitelists
- Crypto validation on request payloads with some secret key
- Header validations

Some services that should be easy to implement with this webhook service are:

- Stripe
- Braintree
- Slack
- GitHub

## Koa

Koa needs some love! 

Here are some internal libraries to Koa that need love:

- https://github.com/crypto-utils/keygrip is a tool for rotating secrets
- https://github.com/pillarjs/cookies is the cookie implementation for Koa

Koa itself needs love with:

- Supporting new node v10 streams
- HTTP2

Contribute! https://github.com/koajs/koa/issues/1114

## My Projects

Here are a bunch of projects of mine that need help:

- https://github.com/jonathanong/ims was going to be a image CMS system
- https://github.com/jonathanong/react-asset-loader should use React Suspense in the future
- https://github.com/jonathanong/s3-proxy-stream
