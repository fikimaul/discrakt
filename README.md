# Discrakt

![Discrakt](./images/demo/discrakt.png)

A simple python script that acts as a bridge between [Discord](https://discord.com/) and [Trakt](https://trakt.tv), allowing for the display of the watch status as [Discord's Rich Presence](https://discord.com/rich-presence).

![User Status](./images/demo/member-list.png)

![Rich Presence](./images/demo/profile-status.png)

## Setup

1. Create an API Application on [Trakt.tv](https://trakt.tv/oauth/applications/new) (with scrobble capabilities) and an Application on [Discord](https://discord.com/developers/applications).
2. Edit the `credentials.ini` file with the required API keys (Cliend IDs) and Trakt username.
3. Upload images, either the ones located in `/images` or ones that you choose to submit (as long as the keys for those images stay `tv` and `movie`) to your Discord RP Art Assets in the [Developer Portal](https://discord.com/developers).
4. Run the respective executable and you're ready to start sharing your progress!

*P.S.* Discord needs to be running on the machine Discrakt is running on. 

## Running executables

Running the executables is as easy as clicking the provided executables in the latest [release](https://github.com/afonsojramos/discrakt/releases) (`.exe` for Windows and `.sh` for UNIX systems). That's it!

## Development

As usual, it is recommended to use [venv](https://docs.python.org/3/library/venv.html) and [Python 3.9](https://www.python.org/). 

After this, simply install the dependencies using `pip install -r requirements.txt`.

### Running from script

After setting things up by following the previous section, you can run this script with: `python discrakt.py`

When a show is detected throught the Trakt API, a similar output is expected in the logs:

![Console](./images/demo/console.png)

In the future, I will provide either a guide or an executable to run this service on boot for both Windows and Linux.

## Thank You

`movie` and `tv` icons by [iconixar](https://www.flaticon.com/authors/iconixar)
