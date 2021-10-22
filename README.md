# Wistia Webhooks Test App

Dependencies: Sinatra, Ngrok, free Wistia account, Pry

## Usage

Run the Sinatra app, preferrably with a single thread for Pry debugger:

```
$ MAX_THREADS=1 ruby app.rb

```

Install/run Ngrok to tunnel to `localhost:4567`:

```
$ brew install ngrok
$ ngrok http 4567

```

Sign up for a free Wistia account. Turn of webhooks in the account settings. Configure a webhook to POST to the Ngrok domain.

E.g., POST URL:
```
https://dbac-97-99-206-201.ngrok.io/wistia/events

```
