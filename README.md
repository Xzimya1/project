# УМНЫЙ ВХОД
мы хотим сделать Вход в школу/другое помещение не прикладывая карту, вывод информации про учеников находящихся в школе. Актуальность данного проекта заключается в том, что карту можно потерять, забыть, оставить дома. Для восстановления карты нужно затрачивать дополнительные средства. В нашем проекте для входа в помещение достаточно лишь фотография вашего лица. Технологии (используемые компоненты) : малинка, ардуинка, серва привод, камера + прочее.В метро существует система распознавания лиц для прохода. Весьма неплохое решение для метро, но эта система имеет несколько недостатков: в московском метро огромное количество станций, благодаря чему система становится достаточно дорогой, хотя в ней почти отсутствует практический смысл. В школах же существуют обычные турникеты к которым нужно прикладывать карточку. Казалось бы простая система, но каждый ученик, каждый день затрачивает время для того чтобы достать карточку из потайного кармана своей сумки/рюкзака/портфеля, чтобы выйти или зайти в школьное учереждение. Также немалой проблемой является человеческий фактор: ученик может потерять, забыть или перепутать карточку, поэтому школе приходится производить затраты на новые карточки, которые выдаются ученикам.
Наша идея заключается в объединении двух устройств: школьных турникетов и "инновационной" системы прохода по лицу в метрополитене. Учебному учреждению больше не придётся затрачивать бюджет на производство/заказ новых карточек для школьников, ведь наша система предполагает вход и выход из помещения учебного заведения, благодаря лицу ученика, преподавателя и так далее.

ИТАК, ЧТО НАМ НУЖНО ИЗ ПЛАТ, ДАТЧИКОВ И ТД?
1)разбери пай(малинка) - есть
2)норальная камера с которой малинка будет считывать изображение - есть но думаю она не пойдет
3)датчик , который будет считвать проход. лазер например - есть
4)серва или моторчик , который открывает проход - есть
прочее будет добавляться сюда по мере нужды / добавлению новых функций

КАК МЫ БУДЕМ РАСПОЗНАВАТЬ ЛИЦО?
https://habr.com/ru/articles/653461/ - вроде тему глаголят
https://proglib.io/p/uchim-raspberry-pi-raspoznavaniyu-lic-2020-11-15 - аналогично
писать будем на питоне (лагишно)
из библиотек:
  OpenCV – это библиотека алгоритмов с открытым исходным кодом для обработки изображений и видео в реальном времени с возможностью машинного обучения;
  Пакет Python face_recognition используется для вычисления ограничительных рамок вокруг лиц, лицевых вложений и сравнения лиц в наборе данных кодирования;
  Imutils – это серия удобных функций для ускорения вычислений OpenCV на Raspberry Pi.
пока вроде все, потом будем добавлять все что нужно

