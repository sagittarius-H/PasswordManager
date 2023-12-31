# Консольный менеджер паролей :lock_with_ink_pen:
Это реализация простого консольного менеджера паролей на языке Python3.<br>

Все пароли сайтов сохраняются в базе данных Sqlite в зашифрованном и засоленном виде.<br>
Шифрование выполняется с помощью симметричного алгоритма AES-128 c мастер паролем, т.е. для добавления или получения любого пароля сайта используется один пароль (мастер пароль). Он задаётся один раз при добавлении самого первого сайта, в дальнейшем для добавления новых сайтов можно использовать только его.
 
**:gear: Сейчас менеджер имеет следующий функционал :gear:**:
* ✏️ Добаление информации для нового сайта и его пароля.
* 🗑️ Удаление сайта и его информации о пароле.
* 📝 Редактирование информации о сайте.
* 🔎 Поиск пароля сайта в базе и вывод его на консоль при правильном вводе мастер пароля.
* 💳 Генерацию паролей заданной длины (минимально 8 символов и >=128).
* ⏱️ Возможность проверять устаревание паролей при поиске. Если пароль был обновлён больше 3х месяцев назад, то пользователю будет выдано предупреждение с рекомендацией обновить пароль сайта.

