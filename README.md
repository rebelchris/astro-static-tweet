# Welcome to Astro Static Tweet 👋

This is a open source [Astro](https://astro.build/) component.
Astro is a open-source Static Site Generator... But it comes with a bring your own framework approach as well as the option to use components but output fully static websites.

So far i'm in ❤️ with [Astro](https://astro.build/).

A small downside I noted when one adds Tweets as embeds to a website, they always pull in JavaScript to render the Tweet.
This makes little to no sense, to just get a fancy like count.

That's why I build this plugin.
You can input a tweet ID and this plugin will convert it into a static tweet!

The best part?
You can even style it 🤫

## Installing the plugin

Once you setup your Astro project simply run the following command:

```bash
npm i @rebelchris/astro-static-tweet
```

You can then use the component like this:

```jsx
---
import { StaticTweet } from '@rebelchris/astro-static-tweet'
---
<StaticTweet id="1359064894377762816" />
```

Now all that's left is for you to get some Twitter credentials, since this plugin uses the Twitter API to fetch the Tweet.

Follow my guide on [getting Twitter credentials](https://daily-dev-tips.com/posts/how-i-made-my-twitter-header-dynamic/) here.

Then create a `.env` file in the root of your project and add the following variables.

```text
TWITTER_API_KEY={API_KEY}
TWITTER_API_SECRET={API_SECRET}
TWITTER_ACCESS_TOKEN={ACCESS_TOKEN}
TWITTER_ACCESS_TOKEN_SECRET={ACCESS_TOKEN_SECRET}
```

And that's it, you're now ready to go!

## Demo

☑️ Sorry, still working on this 😅

## Working on these features

[ ] Fix styling
[ ] Write style guide
[ ] Test all tweet options (media/poll/video/multi image/reaction)
[ ] Enable cache option?
[ ] You tell me? Create an issue with your wishes
