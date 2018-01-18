# github-to-telegram
Simple script to send messages from GitHub callback webhook with payload to telegram api to your group or channel or whatever your want.

All configuration inside `gh-payload.php`

You should configure only two constants:
- `TELEGRAM_BOT_API_KEY` – your telegram bot platform api key received from @BotFather after your bot was created
- `TELEGRAM_CHAT_ID` – your telegram `chat_id` can be found by method https://api.telegram.org/botTELEGRAM_BOT_API_KEY/getUpdates 

Prepared to process events:
- ping
- push (with commits and messages)
- pull_request
- pull_request_review