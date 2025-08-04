# BTC daily monitoring indicator analysis and AI investment advice

Analyze BTC price, AHR999 index, and Fear & Greed index based on historical data, and provide buy/sell recommendations。

## Features

- ✅ Fetch and save BTC historical price data
- ✅ Fetch and parse AHR999 index historical data
- ✅ Fetch Fear & Greed index historical data
- ✅ Analyze market trends based on 6 months of historical data
- ✅ Generate comprehensive investment advice reports integrating multiple indicators
- ✅ Consolidate multiple data sources by date into a unified JSON format
- ✅ Use Deepseek R1 AI model to offer advanced investment analysis suggestions


## Setup
```
- pip install requests pandas python-dotenv
- pip freeze > requirements.txt
- pip install -r requirements.txt
- pip install python-dotenv     # to load environmental variable
- python -m src.alerts.test_telegram_alerts  # run telegram_alerts as a module when imported using "absolute path"
 
 ```



## Alerts
Using `@Botfather` for the telegram notification

Search botfather on telegram 

### How to setup botfather

- Search on BotFather on Telegram
- Open and type `/start` in the chat to generate list of options
- Type in `/newbot` to create a bot
- Create the name of the bot and follow the onscreen instructions
- Copy the Telegram token and chat id. 
    - ```[Token Format]: 4839574812:AAFD39kkdpWt3ywyRZergyOLMaJhac60qc]```
     - Chat id can be found when you run this:
        ``` https://api.telegram.org/bot<TOKEN>/getUpdates ```
 
- Load the telegram token and chat id from env and when sending investment advice


&nbsp;

Below is the implementation of the telegram advisor alert <br>  
![alt text](<Screenshot 2025-08-04 at 8.57.59 PM.png>)

&ensp;
---
MIT License 