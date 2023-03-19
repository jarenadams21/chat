# Chat
 * Elixir chat application to familiarize myself with phoenix & elixir
 * Plan on building additional elixir real-time knowledge off this repo

## Stack
  * Elixir
  * Phoenix Framework
  * Postgre

## Current next Steps
  * Figure out PostgreSQL implementation/installation for DB persistence

## Helpful Reminders
  * Creating a database schema to store chat history
    mix phx.gen.schema Message messages name:string message:string
    <br/>
    mix phx.gen.schema - the mix command to create a new schema (database table)
    Message - the singular name for record in our messages "collection"
    messages - the name of the collection (or database table)
    name:string - the name of the person sending a message, stored as a string.
    message:string - the message sent by the person, also stored as a string.

## Design Justifications
  * We are assuming that most chat apps save history so that new people joining the "channel" can see the history and people who are briefly "absent" can "catch up" on the history.

## Additional/Random Notes & Resources
  * Chat is technically deployable after steps 1-4,
    see -> Anonymous texting app with no history/trace: http://www.psstchat.com/.


To start your Phoenix server:

  * Run `mix setup` to install and setup dependencies
  * Start Phoenix endpoint with `mix phx.server` or inside IEx with `iex -S mix phx.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](https://hexdocs.pm/phoenix/deployment.html).

## Learn more

  * Official website: https://www.phoenixframework.org/
  * Guides: https://hexdocs.pm/phoenix/overview.html
  * Docs: https://hexdocs.pm/phoenix
  * Forum: https://elixirforum.com/c/phoenix-forum
  * Source: https://github.com/phoenixframework/phoenix
