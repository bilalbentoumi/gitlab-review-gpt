# Gitlab ReviewGPT

<p align="center">
  <img src="public/icons/icon_256.png">
</p>
<p align='center'>
    Review Gitlab Merge Requests using ChatGPT so that you can pretent do work.
</p>

## Overview

This is a Chrome extension which reviews Merge Requests for you using [ChatGPT](https://chat.openai.com/).

![example screenshot](/images/screenshot1.png)

## Usage

- Navigate to a Gitlab Merge Request that you want a review for.
- Click the extension icon
- If you have not already, the extension will ask you to log in at [chat.openai.com](https://chat.openai.com)
- You get code review comments from ChatGPT in the popup window

**NB:** Running the review multiple times often produces different feedback, so if you are dealing with a larger MR, it might be a good idea to do that to get the most out of it.
## How to build and install

- Clone this repository `git clone git@github.com:bilalbentoumi/gitlab-review-gpt.git && cd gitlab-review-gpt`
- Install the dependencies `npm install`
- Run the build script `npm run build`
- Navigate to `chrome://extensions`
- Enable Developer Mode
- Click the 'Load unpacked' button and navigate to the `build` directory in the project

## Supported browsers

Currently, only Chrome is supported

## Permissions

This is a list of permissions the extension uses with the respective reason.

- `activeTab` is used to get the URL or the active tab. This is needed to fetch the get the Merge Request details
- `storage` is used to cache the responses from OpenAI

## Credits

This project is inspired by [sturdy-dev/codereview.gpt](https://github.com/sturdy-dev/codereview.gpt)
