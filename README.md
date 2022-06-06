# A WhatsApp Web like (Clone Chat) Application for those developers that like to use Django Channel for handling WebSocket request (Windows Edition)

# inspired from
https://github.com/codingelle/django-whatsapp-web-clone

## Demo For Windows by:
* Me (https://github.com/ManasPhanse)
* Omkar (https://github.com/omkarsalian)
* Mayuri (https://github.com/MayuriSakpal123)
* Kajal (https://github.com/kajolmishra948)

on http://127.0.0.1:8000/admin/

#### Login User1 (Use Chrome Browser)
* Login: manas
* Pass: terna123

#### Login User2 (Use Microsoft Edge or any browser except Chrome)
* User: Mayuri
* Pass: terna123

#### Login User3 (Use Chrome Browser in incognito)
* User: Kajal
* Pass: terna123

#### Login User4 (Use Chrome Browser in guest)
* User: omkar
* Pass: terna123

#### Start Chat
##### Make sure to login using User1 or User2
Group1: http://127.0.0.1:8000/chat/1/
Group2: http://127.0.0.1:8000/chat/4/
Group3: http://127.0.0.1:8000/chat/6/

## Installation
```
cd Msg-App

py -m venv env
env\Scripts\activate
pip install -r requirements.txt

```

## How to run development server?

#### create all the required tables
```
manage.py makemigrations
manage.py migrate
```

#### create superuser
```
manage.py createsuperuser
```

### For Windows, modify settings.py to run Sockets
```
CHANNEL_LAYERS = {
    "default": {
        "BACKEND": "channels.layers.InMemoryChannelLayer"
    }
}
```

### create .env file (for my prj I created key.env)

add the following variable & replace it based on your own development keys
```
API_KEY=YourOwnGiphYAPIKeysdfasjfdgdf

SECRET_KEY=YourOwnSecretKey71041jkfohdslflasdfjhaljdfa
```

#### run the development server
```
manage.py runserver
```
