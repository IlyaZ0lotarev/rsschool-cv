Илья Золотарев

Контакткая информация:
телефон: +79270060042
E-mail: Zolotarev2694@mail.ru
Telegramm: @ilya63xDD
Discord: xdd_163

О себе: 
На текущий момент работаю старшим специалистом по развитию обслуживания в компании одного из ведущих операторов сотовой связи. Занимаюсь написанием и конфигурацией сценариев виртуального помошника. Также есть опыт работы в тестировани. В свободное время
занимаюсь изучением новых для себя технологий. В планах освоить профессию Frontend-разработчика. Увлекаюсь
музыкой, играю на гитаре.

Навыки:
• API
• Git
• Gitlab
• GitHub
• HTML
• YAML
• Jenkins
• Postman
• SQL
• Swagger
• Функциональное тестирование
• Тестирование пользовательского интерфейса

Пример кода:

```python
@bot.message_handler (content_types=['text'])
def get_weather(message):
  city = message.text.strip().lower()
  res = requests.get(f'https://api.openweathermap.org/data/2.5/weather?q={city}&appid={API}&units=metric')
  if res.status_code == 200:
    data = json.loads(res.text)
    temp = data["main"]["temp"]
    bot.reply_to(message, f'Сейчас погода: {temp}°')
  else:
    bot.reply_to(message, f'Город укказан не верно')
```


