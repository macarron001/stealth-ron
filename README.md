# <a href='https://hellostealth.org'><img src='logo.svg' height='120' alt='Stealth Logo' aria-label='hellostealth.org' /></a>

Stealth is a Ruby based framework for creating voice & text chatbots. It's design is inspired by Ruby on Rails's philosophy of convention over configuration. It has an MVC architecture with the slight caveat that `views` are aptly named `replies`.

[![Gem Version](https://badge.fury.io/rb/stealth.svg)](https://badge.fury.io/rb/stealth)
[![CircleCI](https://circleci.com/gh/hellostealth/stealth/tree/master.svg?style=shield)](https://circleci.com/gh/hellostealth/stealth/tree/master)

## Features

* Deploy anywhere, it's just a Rack app
* Variants allow you to use a single codebase on multiple messaging platforms
* Structured, universal reply format
* Sessions utilize a state-machine concept and are Redis backed
* Highly scalable. Incoming webhooks are processed via a Sidekiq queue
* Built-in best practices: catch-alls (error handling), hello flows, goodbye flows

## Getting Started

Getting started with Stealth is simple:

```
> gem install stealth
> stealth new <bot>
```

## Service Integrations

Stealth is extensible. All service integrations are split out into separate Ruby Gems. Things like analytics and natural language processing ([NLP](https://en.wikipedia.org/wiki/Natural-language_processing)) can be added in as gems as well.

Currently, there are gems for:

### Messaging
* [Facebook Messenger](https://github.com/whoisblackops/stealth-facebook)
* [Twilio SMS](https://github.com/whoisblackops/stealth-twilio)
* [Smooch](https://github.com/whoisblackops/stealth-smooch)

### Voice
* [Alexa Skill](https://github.com/whoisblackops/stealth-alexa) (Early alpha)

### Natural Language Processing
* [AWS Comprehend](https://github.com/whoisblackops/stealth-aws-comprehend)

### Analytics
* [Mixpanel](https://github.com/whoisblackops/stealth-mixpanel)

## Docs

You can find our full docs [here](https://hellostealth.org/docs). If something is not clear in the docs, please file an issue! We consider all shortcomings in the docs as bugs.

## License

"Stealth" and the Stealth logo are copyright (c) 2018 The Black Ops Bureau Inc.
