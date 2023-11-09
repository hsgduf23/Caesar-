import telebot
import requests
bot=telebot.TeleBot('6814870328:AAFoh0T0P6x1q8qr9dpJaIETlS2Vjl-8kZY')
@bot.message_handler(commands=['start'])
def ya(message):
 bot.reply_to(message,'welcome to ai chat send your question')
@bot.message_handler(content_types=['text'])
def tah(message):
 i=message.text
 url=f'https://hmss.store/api/chat.php?text={i}'
 r=requests.get(url).text
 bot.reply_to(message,r)
bot.infinity_polling()