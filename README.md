# backend-coding-challenge

The coding challenge is optional if you already have some code on Github that you're proud of and can share with us. If you do, skip to the bottom of this document. 

If you don't already have code to share, you can work on our coding challenge described below 👇.

Please organize, design and document your code as if it were going into production, then send us a link to the hosted repository (e.g. Github, Bitbucket, Gitlab...).

## Technical specs

We believe good engineering is about using the right tool for the right job, and constantly learning about them.

You can **use any web framework**, but here's some of the technologies our teams are familiar with: Python, Javascript, Ruby, PHP, Go, Java, Elixir.

No need to use database or caching system.

## Functional specs

- Develop a REST microservice that list the languages used by the 100 trending public repos on GitHub.
- For every language, you need to calculate the attributes below 👇:
    - Number of repos using this language
    - The list of repos using the language

## How to get Trending Repos from Github

Fetching trending repositories simply translates to fetching the most starred repos created in the last 30 days ( from now ). To do that, you'll need to call the following endpoint:

```
https://api.github.com/search/repositories?q=created:>{date}&sort=stars&order=desc
```

The JSON data from Github will be paginated (you'll receive around 100 repos per JSON page). You can ignore the subsequent pages since you only need the first 100 repositories.

If you want to learn more about the Github API, you can click on the following [link](https://developer.github.com/v3/).


## How we evaluate?

[Read how we review your code](https://www.notion.so/Read-how-we-review-your-code-8581e6a340084c8c924b681ea9790f45)

## Useful links

[Useful links can be found here.](https://www.notion.so/Useful-links-can-be-found-here-112d962342194caaa40f61e1a6a34513)

## Have an existing repo ?

If you have an existing Github repo you can share with us, please reply to our email and share with us the link to your Github repo. Keep in mind that we'll evaluate that repo the same way we review other coding challenge. 

Please make sure you read [how we evaluate your repo](https://www.notion.so/hiddenpole/Read-how-we-review-your-code-413052895a0d4720895c2c433630c8f9).
