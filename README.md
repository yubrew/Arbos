# Arbos

All you need is a Ralph loop and a telegram bot.

## Getting started

```sh
curl -fsSL https://raw.githubusercontent.com/unconst/Arbos/main/run.sh | bash
```

## Next steps

You can ask how the softwar works directly to the bot
```bash
# <prompt>
How do I use you what are your commands
```

The main thing to do is create agents run continously on a ralph-loop. Give them difficult long running problems to chew on.
```bash
# /agent <name> <delay between runs> <prompt>
/agent quant 600 Using my hyperliquid account build out a state of the art quant trading system. 
```

You can send them messages which they get at the beginning of their next loop iteration.
```bash
# /message <name> <message>
/agent quant Lets rewrite our ML architecture using the latest in timeseries foundation models
```

You can give them environment vars to tools
```bash
# /env KEY=VALUE <description>
/env MY_HYPERLIQUID_KEY=******* Use this for trading hyperliquid
```

You do what ever you want by adding features directly. This updates the code and restarts the agent.
```bash
# /adapt <prompt>
/adapt I want you to add a new command /pause <agent> which pauses a running agent
```

