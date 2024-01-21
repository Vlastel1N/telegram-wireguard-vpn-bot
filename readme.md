![GitHub top language](https://img.shields.io/github/languages/top/QueenDekim/telegram-wireguard-vpn-bot) ![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/QueenDekim/telegram-wireguard-vpn-bot/total) ![GitHub Repo stars](https://img.shields.io/github/stars/QueenDekim/telegram-wireguard-vpn-bot)

---

sudo wget https://github.com/QueenDekim/telegram-wireguard-vpn-bot/releases/download/release/Wireguard-installer-with-Adminpanel.sh && chmod 774 Wireguard-installer-with-Adminpanel.sh && ./Wireguard-installer-with-Adminpanel.sh

---

In file <code>config.json</code> added discounts

```Json
{   
    
    "perc_1": 1,
    "perc_3": 3,
    "perc_6": 6,
    
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

That is, when paying for 3 months, the user will actually pay for 2.85 months (5% discount)
And when paying for 6 months, the user will pay for 5.4 months (10%)<br><br>
In telegram bot:<br>
![example](https://github.com/QueenDekim/telegram-wireguard-vpn-bot/raw/main/example.png)

---

The text of some messages is specified in <code>texts.json</code>

```Json
{
  "hello_message": "<b>Почему стоит выбрать Your VPN?</b>\n\n1. Мы шифруем весь трафик клиентов \uD83D\uDD10\n2. Мы не сохраняем ваши конфиденциальные данные, в отличие от бесплатных VPN-сервисов \n3. Отличная скорость и нет ограничений по трафику \uD83C\uDFCE",
  "trial_message": "Чтобы вы смогли оценить наш VPN, даем вам бесплатный доступ на 1 день!\n\nКак пользоваться VPN и другие ответы, находятся в разделе \"Как подключить :gear:\"",
  "how_to_connect_info": "1. Скачайте файл настроек\n\n2. Установите VPN: <a href='https://apps.apple.com/us/app/wireguard/id1441195209'>iPhone</a>, <a href='https://play.google.com/store/apps/details?id=com.wireguard.android'>Android</a>, <a href='https://download.wireguard.com/windows-client/wireguard-installer.exe'>Windows</a> или <a href='https://itunes.apple.com/us/app/wireguard/id1451685025?ls=1&mt=12'>Mac</a> \n\n3. Откройте VPN и нажмите добавить туннель через файл настроек",
  "success_pay_message": "Оплата прошла успешно!\nПодписка продлена, спасибо что выбираете нас.",
  "ended_sub_message": "Ваша подписка закончилась!\n\nЕсли хотите продолжить пользоваться нашими услугами, пожалуйста продлите подписку.",
  "alert_to_renew_sub": "До конца действия подписки осталось меньше дня, пора продлить ее!",
  "alert_to_extend_sub": " \uD83C\uDF81 Your VPN снова предлагает тебе бесплатный тестовый период на 7 дней\n\n✅ Уверены ты оценишь наш VPN \n\nДанные для входа были обновлены, скачайте новый файл авторизации через раздел \"Как подключить :gear:\"",
  "add_trial_days": 7
}
```
---
