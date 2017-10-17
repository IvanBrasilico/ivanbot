Bottery test application.
Needs bottery installed (Currently my version).

Installing:

```
git clone https://github.com/IvanBrasilico/ivanbot.git
cd ivanbot
git clone https://github.com/IvanBrasilico/bottery.git
mv bottery bottery_core
ln -s bottery_core/bottery bottery 
```

Running:

First create a bot on https://telegram.me/botfather

Then create a settings.py archive with your token:
```
HOSTNAME = ''

PLATFORMS = {
    'telegram': {
        'ENGINE': 'bottery.platform.telegram',
        'OPTIONS': {
            'token': '@BotFather:will_give_you_a_token',
        }
    },
}
```

Now you can run your bot:

```
python3 app.py
```
