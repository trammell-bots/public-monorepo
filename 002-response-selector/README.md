Simple chitchat bot to play with; see
[response selectors](https://rasa.com/docs/rasa/chitchat-faqs/).

## Warnings

Validating the bot data with `rasa data validate` and training this bot with
`rasa train` yield this warning:

```
UserWarning: The following duplicated intents have been found across multiple
domain files: chitchat
More info at https://rasa.com/docs/rasa/domain
```

This warning is spurious; apparently the structure of response selectors looks
like duplicate intents?

