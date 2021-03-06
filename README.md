# filetolinktg

demo : [@HYBRID_F2L_BOT](https://t.me/HYBRID_F2L_BOT)


# Run :

* Docker :

    > install docker , docker-compose
    
    > set Environment or edit Config/__init__.py
    
    `docker-compose up`

* Heroku :

    [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/zainulhibath/filetolinktg)

    `git clone https://github.com/zainulhibath/filetolinktg`
    
    > edit Config/__init__.py
    
    `heroku create` or `heroku git:remote -a appname`
    
    `git push heroku master`

* Cli :

    > install python3.8+
    
    `git clone https://github.com/zainulhibath/filetolinktg`
    
    > set Environment or edit Config/__init__.py
    
    `pip install -r requirements.txt`
    
    run web : 
        `gunicorn main:main --workers 4 --threads 4 --bind 0.0.0.0:$PORT --timeout 86400 --worker-class aiohttp.GunicornWebWorker`
        
    run bot :
        `python -m bot`
        
    run web and bot :
        `./start`


Environment :
|env|description|Example|
|-|-|-|
|api_id|api_id Telegram to develop a robot to receive my.telegram.org|12345|
|api_hash|api_hash Telegram to develop a robot to receive my.telegram.org|21ab7cb0a453b5e60016dc7bbeb701cb|
|channel_files_chat_id|Telegram channel chat ID for storing and managing files|-10012345466|
|channel_username|Telegram channel username for support|Userlandapp|
|token|Telegram robot token for launch|0000000:AAFFMMgYoL9Vjb5KUU0bXxVReUI81xuU|
|domain|application domain|https://hybridf2l.herokuapp.com|



Management guide:

    If a file is deleted from the storage channel, the link will expire
    If a file is replayed in the storage channel and a message is sent, that message will be sent to the sender of the file
    If a file is edited in the storage channel and replaced by another file, the link will download the new file
    If a user is blocked from the support channel, he can no longer use the robot


## Support Telegram Group and Channel

<a href="http://t.me/Tech_MasterZ"><img src="https://smartiblogster.com/wp-content/uploads/2021/03/smartiblogster-iblogster-join-telegram-channel.png" style="width: 300px; height: 100px"></a>

<a href="http://t.me/Tech_MasterZ_Chat"><img src="https://www.pngitem.com/pimgs/m/214-2144731_groups-on-telegram-telegram-group-link-png-transparent.png" style="width: 280px; height: 80px"></a>
