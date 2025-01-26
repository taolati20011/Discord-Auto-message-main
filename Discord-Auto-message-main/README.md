# Discord Auto Messenger

This Python script enables automated messaging in a Discord channel, enhancing the experience by sending messages from a chat dataset to mimic human-like behavior.

## Installation

### Local Machine

1. Clone the repository or download the code as a zip file and extract it to a folder.
2. Navigate to the project directory in your terminal:

    ```
    cd /Downloads/Discord-Auto-message/
    ```

3. (Optional) Customize the message content by editing **messages.txt**, adding messages on separate lines. By default, random messages are provided.

## Usage

Execute the script using the following command:

```
python auto.py
```

During execution, you'll be prompted to specify the duration in seconds between each message and the sleep interval after each cycle.

## Options

The script offers the following options:

`--config`: Configure user information by providing user ID, Discord token, Discord channel URL, and Discord channel ID:

```
python auto.py --config
```

`--setC`: Set the channel for message delivery by providing the Discord channel URL and channel ID:

```
python auto.py --setC
```

`--help`: Display help information for the script and its available options:

```
python auto.py --help
```

## Formatting

Your info.txt file must following this:

```
{discord_id}
{Authorization}
{Channel URL}
{Channel ID}
```

## How to get info

1. Discord_id

Open discord setting, go to Advanced (in App Settings) -> Turn on Developer Mode
-> Back to My Account tab, click on `...` -> Copy User ID

2. Authorization header

Open url: `https://discord.com/channels/@me` on web, log in to your discord
-> Open F12 tab (inspect mode) -> In Network tab (Logo wifi), find request with name `2`
-> Look to the right, in Header tab, find Authorization header

3. Channel URL

Right click on the channel and click Copy Link

4. Channel ID

Right click on the channel and click Copy Channel ID

## First time using step

1. Run command

```
python auto.py
```

Enter your config (info.txt)

2. Edit messages.txt file

This code will auto chat one line message in messages.txt file, you can remove or add new message

