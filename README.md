# TestApp

**This is a barebones example application that demonstrates how to embed
multiple SPAs (Single Page Applications) within a phoenix app.**

To start your Phoenix app:

  1. Install dependencies with `mix deps.get`
  2. Create and migrate your database with `mix ecto.create && mix ecto.migrate`
  3. Start Phoenix endpoint with `mix phoenix.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

## Learn more

  * Official website: http://www.phoenixframework.org/
  * Guides: http://phoenixframework.org/docs/overview
  * Docs: http://hexdocs.pm/phoenix
  * Mailing list: http://groups.google.com/group/phoenix-talk
  * Source: https://github.com/phoenixframework/phoenix

# Ember SPAs

While you have your phoenix server running, you can develop your apps located in
`/apps` as you wish, for this example ember.js with `ember-cli` is used.

When you're done developing features, type
`ember build --environment="production`. This command compiles your app to a
folder with an `index.html` and a few assets and moves this folder to
`/web/static/assets`. Phoenix will copy all files/folders
in `/web/static/assets` as-is to `priv/static`, where it gets finally served
from.