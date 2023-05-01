Simple chitchat bot to play with; see
[response selectors](https://rasa.com/docs/rasa/chitchat-faqs/).


## Warnings

Training this bot yields this warning:

```
UserWarning: The following duplicated intents have been found across multiple domain files: chitchat
More info at https://rasa.com/docs/rasa/domain
```

This warning is spurious; apparently the structure of response selectors looks
like duplicate intents?

I feel like the training code could be smart enough not to emit this warning
when it knows it's working with response selectors.

