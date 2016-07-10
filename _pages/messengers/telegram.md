---
layout: default
title: Telegram
permalink: /messengers/telegram/
---

Zenbot implements [Telegram](https://telegram.org) bot API, so you do not have to have an external hosting to make your natural language speaking bot for Telegram.
Just provide your Telegram\'s bot Authorization token in Zenbot\'s bot settings, and it will start speaking with your users over Telegram.

## How to create Telegram bot
There is a [complete guide](https://core.telegram.org/bots#3-how-do-i-create-a-bot) about how to create Telegram bot and obtain it\'s Authorization token.

Just provide this token in your Zenbot\'s bot Telegram settings.

![Telegram settings](/img/telegram.png)

## Test your Telegram bot
Select your bot in Telegram and send a text message.
Your bot will respond with text responses regarding the [Botscript](/botscript/).

Note that telegram can also interpret HTML tags in responses.
Thus your bot can respond with HTML links and Telegram will load snippets of web pages on fly in chat window.

## Start message
Each time user presses "Start" button in Telegram messenger client, your bot will receive "/start" message following by some payload it was provided.

Thus you have to provide `/start $Text` input pattern in your Botscript if you need to response to the start command.

## Response formatting
Please use a [Markdown formatting](https://core.telegram.org/bots/api#markdown-style) in each response of your bot if you wish to format a text with bold, italic, pre-formatted or insert any URL links.

{% include note.html text="Note that you must enclose each URL link in [] and ()" %}

## Botan analytics
Zenbot currently supports a [Botan analytics](http://botan.io/) service API to track your Telegram bot\'s statistics.

This service enables your bot to store it\'s analytics data automatically for each user\'s request.
Further you can track bot\'s metrics through a [special Botan bot](https://telegram.me/Botaniobot?start=src%3Dbotanio) in Telegram.

To enable Botan integration for your bot, just obtain a Botan token and provide it through the [web console](https://zenbot.org) in the "Telegram settings" section.

{% include note.html text="Note that Zenbot will track only identifiers of inputs.
So if the matched input has not an \"id\" attribute, it will not be tracked." %}

## Variables
Each time Zenbot receives a request from Telegram, it produces a set of special variables.

- `req_telegram_token` - your Telegram bot Token
- `req_telegram_chat` - current Telegram chat identifier
