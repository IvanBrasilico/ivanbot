Bottery test application.
Needs bottery installed (Currently my version).

Install and run:

git clone https://github.com/IvanBrasilico/ivanbot.git

cd ivanbot

git clone https://github.com/IvanBrasilico/bottery.git

mv bottery bottery_core

ln -s bottery_core/bottery bottery 


Create a bot on https://telegram.me/botfather

create a settings.py archive:

"""HOSTNAME = ''

PLATFORMS = {
    'telegram': {
        'ENGINE': 'bottery.platform.telegram',
        'OPTIONS': {
            'token': '@BotFather:will_give_you_a_token',
        }
    },
}"""

RUN:
#python3 app.py
