# Slack勤怠ボタン

Button to report attendance to slack
- Supports multiple workspaces and multiple channels.
- Record the time.
- There are only the minimum functions necessary for me.


<img src="images/preview.png" width="300">

<img src="images/results.png" width="300">


## Installation

- Clone or Download this repository.
- Copy `config.js.dist` to `config.js`.
- Change parameters in `config.js` as described in the comments.
  - *Highly Recommend* : First, test on your personal test channel. 

## Slack App Setup

1. Go to [Slack API](https://api.slack.com/apps) and click "Create New App"
2. Choose "From scratch" and set up app name and workspace
3. In the "OAuth & Permissions" section, add the following scopes:
   - `chat:write`
   - `chat:write.public`
4. Click "Install to Workspace" to install the app
5. Copy the displayed "Bot User OAuth Token" (starting with `xoxb-`)
6. Set this token in your `config.js` file in the `target_list`

## Getting Thread IDs

- Get thread_ts from message.
  - <img src="images/thread_ts_1.png" width="300">
  - <img src="images/thread_ts_2.png" width="300">
  - Get `thread_ts` parameter value from query string.


## Usage

1. Open index.html. (Recommended to put in "Favorites" or create an alias on your desktop)
2. Press the button!
