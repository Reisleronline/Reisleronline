- 👋 Hi, I’m @Reisleronline
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Reisleronline/Reisleronline is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
if kisi.user.is_bot == False:
                    isim = kisi.user.first_name
                    app.send_message(message.chat.id,f"[{isim}](tg://user?id={kisi.user.id}) {metin}")
                    time.sleep(2)

                    sayac += 1
                    if sayac == sayi:
                        app.send_message(message.chat.id,f'{sayi} Kişi Etiketlendi...\nby @ReislerSupport')
                        break


    else:
        metin = ""
        for i in message.text.split()[1:]:
            metin += i + ' '
        sayi = 50
        sayac = 0
        kisiler = app.get_chat_members(message.chat.id)


        message.reply(f"Kişiler etiketleniyor...\n**Sebep** : {metin}\n**by** __@ReislerSupport")

        for kisi in kisiler:
            if kisi.user.is_bot == False:
                isim = kisi.user.first_name
                app.send_message(message.chat.id, f"[{isim}](tg://user?id={kisi.user.id}) {metin}")
                time.sleep(2)

                sayac += 1
                if sayac == sayi:
                    app.send_message(message.chat.id, f'Kişiler Etiketlendi...\nby @ReislerSupport')
                    break


app.run()

{
    "_": "Message",
    "message_id": 592,
    "from_user": {
        "_": "User",
        "id": 1617782127,
        "is_self": false,
        "is_contact": false,
        "is_mutual_contact": false,
        "is_deleted": false,
        "is_bot": false,
        "is_verified": false,
        "is_restricted": false,
        "is_scam": false,
        "is_fake": false,
        "is_support": false,
        "first_name": "Adsız Kaptan",
        "status": "recently",
        "username": "kizilsancaksahibi",
        "language_code": "tr",
        "dc_id": 4,
        "photo": {
            "_": "ChatPhoto",
            "small_file_id": "AQADBAADZroxGz2-8FMACK0onyddAAMCAANvZW1gAATIUy9Ey-fIzJdqBwABHgQ",
            "small_photo_unique_id": "AQADrSifJ10AA5dqBwAB",
            "big_file_id": "AQADBAADZroxGz2-8FMACK0onyddAAMDAANvZW1gAATIUy9Ey-fIzJlqBwABHgQ",
            "big_photo_unique_id": "AQADrSifJ10AA5lqBwAB"
        }
    },
    "date": "2021-04-21 06:08:49",
    "chat": {
        "_": "Chat",
        "id": -1001343550284,
        "type": "supergroup",
        "is_verified": false,
        "is_restricted": false,
        "is_creator": false,
        "is_scam": false,
        "is_fake": false,
        "title": "REİSLER ONLİNE",
        "permissions": {
            "_": "ChatPermissions",
            "can_send_messages": true,
            "can_send_media_messages": true,
            "can_send_stickers": true,
            "can_send_animations": false,
            "can_send_games": true,
            "can_use_inline_bots": true,
            "can_add_web_page_previews": true,
            "can_send_polls": true,
            "can_change_info": true,
            "can_invite_users": true,
            "can_pin_messages": true
        }
    },
    "mentioned": false,
    "scheduled": false,
    "from_scheduled": false,
    "text": "@all",
    "outgoing": false,
    "command": [
        "all"
    ]
}
