# 🎵 Square JMusicBot
## Host JMusicBot (Discord Music Bot) on Square Cloud ☁️

> 🌐 Easily host your own Discord music bot on Square Cloud and play music in your Discord server, right from the cloud.

> [!WARNING]
> Since March 2026, Discord requires [DAVE](https://daveprotocol.com/) (end-to-end encrypted voice) to join voice channels. JMusicBot 0.4.3, the latest release of the [JMusicBot project](https://github.com/jagrosh/MusicBot), does not support DAVE, so **the bot logs in but cannot join voice channels**. To host music for your bot today, use our [Lavalink project](https://github.com/squarecloud-education/lavalink-web) with a Lavalink client library that supports DAVE.

---

## 🚀 How to host this project on Square Cloud

New to Square Cloud? Follow these steps in order. You will create an account, choose a plan, create your bot on Discord and upload a ready-made zip.

### 1️⃣ Create your Square Cloud account

Sign up on the [Square Cloud signup page](https://squarecloud.app/en/signup) with your email.

### 2️⃣ Choose a plan

Hosting on Square Cloud requires an active plan, and the upload in step 5 asks for one, so choose it now.

JMusicBot needs **1 GB of RAM**: the **[Hobby plan](https://squarecloud.app/en/pricing)** runs it. Compare every plan and its price on the [pricing page](https://squarecloud.app/en/pricing).

### 3️⃣ Create your bot on Discord

1. In the [Discord Developer Portal](https://discord.com/developers/applications), click **New Application** and give it a name.
2. On the **Bot** tab, click **Reset Token** and copy the token. Keep it secret: it controls your bot.
3. On the same tab, under **Privileged Gateway Intents**, turn on **Server Members Intent** and **Message Content Intent**.
4. Invite the bot to your server: on **OAuth2 > URL Generator**, check `bot`, choose its permissions and open the generated link.

### 4️⃣ Download the project

Download **`project.zip`** from the [latest release](https://github.com/squarecloud-education/music-bot/releases/latest). This is the file you upload in the next step: you don't need to extract it.

### 5️⃣ Upload it to Square Cloud

1. Open the [Square Cloud upload page](https://squarecloud.app/en/dashboard/new).
2. Select the **zip** option and send the `project.zip` you downloaded.
3. Open **Advanced configuration** and add these environment variables:
   - `BOT_TOKEN`: the token from step 3
   - `BOT_OWNER_ID`: your Discord user ID (turn on **Developer Mode** in Discord's **Advanced** settings, right-click your name and choose **Copy User ID**)
   - `PREFIX`: the command prefix, for example `!`
4. Click **Deploy**.

![Uploading a project to Square Cloud](https://cdn.squarecloud.app/docs/articles/dashboard/uploading.gif)

### 6️⃣ Test it

In your Discord server, send `!help` (with your prefix) to see the bot's commands. If it doesn't answer, open your application in the [Square Cloud dashboard](https://squarecloud.app/en/dashboard) and check its logs.

📖 Need more details? Read the [Discord bot guide](https://docs.squarecloud.app/en/tutorials/bots/discord) in the Square Cloud documentation.

---

## 📚 About the project

The goal of this project is to let you host a Discord music bot on Square Cloud, so you can play music in your Discord server from anywhere, directly from the cloud.

---

🙋‍♂️ **Questions or suggestions?** Contact [Square Cloud Support](https://squarecloud.app/sac) or open an issue in this repository!

---

## 🙏 Credits

Maintained by [@JoaoOtavioS](https://github.com/JoaoOtavioS) on GitHub.
