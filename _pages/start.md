---
layout: default
title: Getting started
permalink: /start/
---

Well, there was a good [introduction](/) and now it is time to get closer to Zenbot.

# What Is Zenbot
Zenbot is an online _natural language processing_ (NLP) service and bot hosting.

It enables you to add a natural language interface to any application, website or chatbot for widely used messengers like Facebook, Slack, Skype and Telegram.

<div style="background-color: #000; padding: 20px; color: #fff; min-height: 400px">
<img src="/img/doit_mockup.gif" width="199" height="368" style="margin: 10px" align="right">

<h2>Natural Language Interface?</h2>
<p>Yep! The era of artificial intelligence and advanced human-to-computer interfaces is already here!</p>
<p>Zenbot makes it really easy to upgrade your bot or application so <i>it can understand</i> the user’s text or voice input.</p>

<h2>Where to Use It?</h2>
<p>Strictly speaking, you can use this ability everywhere instead of large forms, overloaded interfaces, bunches of buttons and checkboxes and other UI components.</p>
<p>Also there are some areas where the user’s voice is one of the most appropriate choice for human-to-machine interface. 
Like smart homes, automotive applications, wearable devices, and yes — <b>chatbots</b>!</p>
</div>

# How Does It Work?
You have to create a [Botscript](/botscript/) (a simple XML formatted file) and upload it to Zenbot through [web console](https://zenbot.org).

Zenbot creates a bot from your Botscript and proceeds all text requests to your bot managing conversation, context understanding, entity extraction and all other AI stuff.

You can also provide some code in your Botscript, so Zenbot can compute it "on-the-fly" while processing a request.
Thus you can request some external service\'s REST API, calculate some variable\'s value and so on _right inside your bot_!

As a result, Zenbot generates some text output and a bunch of resulting [variables](/vars/variables/) you can use on your side if you need.
And the next request will be processed by Zenbot through the extended context with bunch of previously calculated variables in memory.

{% include note.html text="Note that you do not have to have any external servers or databases! Zenbot hosts all your bots by itself." %}

### More than a "pattern matcher"
Based on the pattern matching concept, Zenbot is not limited with this feature only.

Zenbot enables you to build a _conversational_ bots though the idea of [extendable conditional contexts](/botscript/conversations/).

Also Zenbot performs named _entity extraction_ and provides a simple way to store and operate with a big data in your patterns through [custom entities](/pattern/entities/) (like cities names).

And moreover, Zenbot performs not only an NLP and AI stuff - it also allows you to evaluate some [Javascript code](/vars/javascript/) right on the Zenbot\'s side to calculate variable values.

## Messengers Integration, REST API and Telephony
You can use Zenbot’s [REST API](/rest/) to process any text or speech input in your own application or website through a Zenbot\'s NLP engine and build a conversations.

Also Zenbot is already integrated with such popular messengers as [Facebook Messenger](/messengers/facebook/), [Slack](/messengers/slack/), [Skype](/messengers/skype/), [Telegram](/messengers/telegram/), [Kik](/messengers/kik/) and [WeChat](/messengers/wechat/)!
So you can easily spread your bot over these platforms to make your service available as a chat bot for millions of customers!

And moreover - you can use a telephony channels to robotize your call-center with [Voximplant integration](/telephony/voximplant/)!

{% include note.html text="And once again — you do not have to implement all these messengers API and host such implementation on external servers! Zenbot takes care about this for you. All you need is to provide settings for each messenger platform through Zenbot web console." %}

# How to Start
As you will see, there are no additional requirements to you before you can start using Zenbot.
All you have to do is to [read about Botscript](/botscript/) and imagine how your users would converse with your app or chat bot.

The next point is to [read about Zenbot features](/features/) and [have a look at some examples of Botscripts](/samples/) and start creating your own new awesome bot!

When you’re done, just upload your Botscript through [Zenbot web console](https://zenbot.org) and test it.