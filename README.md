# RSS-GPT

![](https://img.shields.io/github/last-commit/yinan-c/RSS-GPT/dev?label=updated)
[![](https://img.shields.io/github/actions/workflow/status/yinan-c/RSS-GPT/cron-job.yml?label=cron-job)](https://github.com/yinan-c/RSS-GPT/actions/workflows/cron-job.yml)
[![](https://img.shields.io/github/actions/workflow/status/yinan-c/RSS-GPT/jekyll-gh-pages.yml?label=GitHub%20Pages)](https://github.com/yinan-c/RSS-GPT/actions/workflows/jekyll-gh-pages.yml)
![](https://img.shields.io/github/stars/yinan-c/RSS-GPT)


[Configuration Guide](https://yinan-c.github.io/rss-gpt-manual-en.html) | [中文介绍](README-zh.md) | [中文教程](https://yinan-c.github.io/rss-gpt-manual-zh.html)

## Features

- Use ChatGPT to summarize RSS feeds, and attach summaries to the original articles, support custom summary length and target language.
- Aggregate multiple RSS feeds into one, remove duplicate articles, subscribe with a single address.
- Add filters to your own personalized RSS feeds.
- Host your own RSS feeds on GitHub repo and GitHub Pages.

![](https://i.imgur.com/7darABv.jpg)

## Quick configuration guide

- Fork this repo
- Add Repository Secrets
    - U_NAME: your GitHub username
    - U_EMAIL: your GitHub email
    - WORK_TOKEN: your GitHub personal accesstoken with `repo` and `workflow` scope, get it from [GitHub settings](https://github.com/settings/tokens/new)
    - OPENAI_API_KEY(OPTIONAL, only needed when using AI summarization feature): Get it from [OpenAI website](https://platform.openai.com/account/api-keys)
- Enable GitHub Pages in repo settings, choose GitHub Actions as the source
- Configure your RSS feeds in config.ini

You can check out [here](https://yinan-c.github.io/rss-gpt-manual-en.html) for a more detailed configuration guide.

## ChangeLog and updates

- There is a [`dev` branch](https://github.com/yinan-c/RSS-GPT/tree/dev) for manual updates on the script, auto commits will no longer be pushed to this `dev` branch. The purpose of doing this is to separate the manual updates and auto commits, so that it is easier to check the updates and pull to your repo.
- Check out the [CHANGELOG.md](CHANGELOG.md).

## Example feeds being processed

These feeds on hosted in the [`doc/` subdirectory](https://github.com/yinan-c/RSS-GPT/tree/main/docs) in this repo as well as on my [GitHub Pages](https://yinan-c.github.io/RSS-GPT/). Feel free to subscribe in your favorite RSS reader.

I will consider hosting more feeds in the future. Email me or submit an issue if there is any question using the script or any suggestions.
- http://www.v2ex.com/index.xml -> https://hzcy.github.io/RSS-GPT/v2ex.xml
- http://www.hostloc.com/forum.php?mod=rss&fid=45&auth=0 -> https://hzcy.github.io/RSS-GPT/hostloc.xml
- http://free.apprcn.com/feed/ -> https://hzcy.github.io/RSS-GPT/apprcn.xml
- https://rsshub.app/gcores/category/news -> https://hzcy.github.io/RSS-GPT/gcores.xml
