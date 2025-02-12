
#### Features:

- Inline query to start the game.
- PvP - play with friends.
- Bot works in any group or private chat.
- All moves stored in the DB, so you can play a few games simultaneously.

**[Demo]**(https://t.me/chessy_bot) (WIP version)

## Usage

To play chess simply type `@chessy_bot[SPACE]` to your telegram message input box.

![](img/3.png)

Then choose a side you want to play with. You will see an inline message with a chess board and a **"Join to game"** at the bottom.

![](img/4.png)

When someone join your game, this will be displayed in the status message. Also the **"Join to game"** button will become **"Settings"**.

![](img/5.png)

Now everything is ready to start the game. To move your pieces just select a piece you want to move and then select a destination from displayed available to move squares.

> **WARNING!!!**
>
> The board is rotating each turn by default! The active player always placed at the bottom!

## Install and run own bot instance

First clone this repository and install dependencies. Run in the terminal:

```bash
git clone git@github.com:Piterden/chessbot.git
cd chessbot
npm i
```

Then you have to create and fill up a new `.env` file:

```bash
cp .env.example .env
editor .env
```

Next migrate the DB:

```bash
npm run knex migrate:latest
```

Then run the dev mode:

```bash
npm run dev
```

)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
