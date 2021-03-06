# Mastodon Broadcaster

![](mastodon-broadcaster.png)

Broadcasts your toots to the world.
Written in NodeJS.

Multiple accounts supported.

## Supported networks

- Twitter

## Installation

Clone

```bash
git clone https://github.com/superevilmegaco/node-mastodon-broadcaster
```

Change into cloned dir

```bash
cd node-mastodon-broadcaster
```

Install dependencies

```bash
# With yarn
yarn

# or with npm
npm install
```

## Configuration

Copy `config.js.dist` to `config.js` and edit the values accordingly.

```bash
cp config.js.dist config.js && vim config.js
```

If you don't have an Twitter App ID yet,
create one [here](https://apps.twitter.com/app/new).

## Start the *daemon*

Run the script forever with `forever`

```bash
nohup node_modules/.bin/forever app.js >> log/error.log &
```

## Stop the *daemon*

```bash
nohup node_modules/.bin/forever stop app.js
```

