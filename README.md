# GitGram Self-hosted
[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/pokurt/GitGram)

This repository is where the self-hosted, private instance version of GitGram lives. It uses plain webhooks and PTB to receive repository
activity and send it to your groups or to your PMs.

If you ever come here to kang our source code, no support will be given unless you requested to assist you to fix license
issues. Otherwise, instant ban will be given to you without any further notice.

## Setup:
- Install all requirements with `pip3 install -r requirements.txt`
- We recommend to use environment variables to configure your instance. To use it, set `ENV` to `True` and
then cofnigure `APP_URL`, `BOT_TOKEN`, `GITGRAM_SUPPORT`, `GIT_REPO_URL`, and `PROJECT_NAME` variables.
    - If you prefer the old way, edit your `config.py`, but DO NOT COMMIT!
- Run `python3 GitGram.py`

## Deploy on Heroku:
If you want to deploy this app on Heroku, there's a one-click setup for that. Click below, fill up the form and hit **Deploy App**.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

### Prefer to use Auto-Deploy?
Bruh, want to be like [the Pins team](https://t.me/ThePinsTeam_GitGramBot)'s instance or can't install `heroku` CLI?

- Fork this repository, as you would do with other repos.
- Sign in to Heroku and create a new app.
- Open your app's overview. Under **Deploy** tab, select **Deployment method** to `GitHub`, connect your repo
- Select `master` to enable auto-deploys.
- Then on **Settings** tab, add `APP_URL`, `BOT_TOKEN`, `GITGRAM_SUPPORT`, `GIT_REPO_URL`, and `PROJECT_NAME` variables. To use them, set `ENV` to `True`.
- Just one restart away to run your instance. To setup, open your bot's PMs or add it to your group and use `/connect` command.

## Try on Gitpod:
1. [Login to Gitpod](https://gitpod.io/login).
2. [Open this repo in Gitpod](https://gitpod.io/#github.com/pokurt/GitGram).
3. After workspace build, dependencies will be installed.
4. Configure your bot and then start the server.
