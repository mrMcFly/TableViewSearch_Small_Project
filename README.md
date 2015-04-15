
Задание:

Level 1.
- Создайте класс студента. У него должны быть свойства: имя, фамилия и год рождения.
- Генерируйте случайное количество студентов и отобразите их в вашей таблице (слева имя и фамилия, а справа дата рождения).

Level 2.
- Сгрупируйте студентов по секциям годов рождения.
- Внутри секции студенты должны быть отсортированы по имени по алфавиту, а если имена одинаковы, то и по фамилии.
- Добавьте индекс бар для быстрого перехода по секциям.

Level 3.
- Добавьте серчбар как в видео, чтобы кнопочка кенсел анимировано добавлялась/уезжала и тд.
- Фильтруйте студентов каждый раз, когда вводится новая буква, причем совпадения ищите как в имени так и в фамилии.

Level 4.
- Добавьте к серчбару сегментед контрол с тайтлами: Год рождения, Имя, фамилия (по умолчанию включен год рождения).
- Когда пользователь переключает сегментед контрол, то секции меняются на соответствующие. Например если выбран контрол с именем, то студенты должны быть отсортированы по имя-фамилия-дата, и должны быть собраны в секции, соответствующие первой букве имени.
- То же самое и для фамилий, фильтр = фамилия-дата-имя если выбрана дата, то все должно отсортироваться как в начале.

Дополнительно:
- Создание секций происходит не в main потоке,а при помощи классов NSBlockOperation и NSOperationQueue.
- При нажатии на ячейку студента отображается детальная информация (Картинка,имя,фамилия,год рождения,уникальная фраза).
- В случае,если последовательность символов с секции поиска не соответствует последовательности в имени или фамилии,тогда выводится предупреждение (объект класс UIAlertController),и строка поиска возвращается в последнюю valid последовательность.
- Создание constarints для всех типов устройств.