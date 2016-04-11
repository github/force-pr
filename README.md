# Force Pull Requests

Just a basic webserver that responds to webhooks with success. This allows you to protect a branch and prevent users from pushing into master without a Pull Request.

## Configuration

* Create a GitHub access token with `repo-status` permissions
* Set `GITHUB_TOKEN` to the token you created 
* Then add a webhook to the server `[hostname]/payload` for `push` events.

![](https://cloud.githubusercontent.com/assets/35968/13334352/70abe0c0-dbc0-11e5-8f95-dad1faecf1c0.png)

You'll then see Pull Requests return successful

![](https://cloud.githubusercontent.com/assets/35968/13303959/0735018a-db07-11e5-978e-693fe7b311db.png)
