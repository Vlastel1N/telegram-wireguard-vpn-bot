
---
<h1 align=center>Recommended Ubuntu (Debian) version - from 14.04 to 22.04</h1>

on versions higher than 23, installation may not complete correctly

---
<h1 align=center>This is fork of <a href="https://github.com/svishnevskii/telegram_wireguard">svishnevskii/telegram_wireguard</a> repositry</h1>

---
<h2>Quick installation:</h2>

```bash
sudo wget https://github.com/QueenDekim/telegram-wireguard-vpn-bot/releases/download/release/Wireguard-installer-with-Adminpanel.sh && chmod 774 Wireguard-installer-with-Adminpanel.sh && ./Wireguard-installer-with-Adminpanel.sh
```
- after configuring the wg, a choice will appear: `Hotite li ustanovit' srazu Telegram bota(1 - Da, 0 - Net):` We agree (press 1)
- Then we specify the `Telegram API` of the bot, which we received from **BotFather** when creating the bot, `YooKassa key shop `, which we also received from **BotFather** when setting up the Payment of the bot and `Telegram-id Admin` - your telegram account ID

<h3>Сhecking the operation of the service</h3>

```bash
sudo systemctl status befutureAdmin
```

<h3>Start</h3>

```bash
sudo systemctl start befutureAdmin
```

<h3>Stop</h3>

```bash
sudo systemctl stop befutureAdmin
```

<h3>Restart</h3>

```bash
sudo systemctl restart befutureAdmin
```

---

<h2>In file <code>config.json</code> added discounts</h2>

```Json
{   
    "...":"...",
    "perc_1": 1,
    "perc_3": 3,
    "perc_6": 6,
    "...":"...",
}
```

We specify the number of months for which the user will actually pay (interest is calculated automatically)<br>
For example:
<code>config.json</code>

```Json
{
    "admin_tg_id": "",
    "one_month_cost": 500,
    "trial_period": 2,
    "perc_1": 1,
    "perc_3": 2.85,
    "perc_6": 5.4,
    "UTC_time": 3,
    "tg_token": "",
    "tg_shop_token": ""
}
```

