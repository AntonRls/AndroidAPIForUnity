# AndroidAPIForUnity
Android API для Unity

В этом репозитории находится плагин для использования Android API в Unity

**Документация**

Все методы вызываются через AndroidAPI

Toas(string message) - вызывает всплывающее окно. Имеет атрибут типа string, который отвечает за показываемое сообщение
AndroidAPI.Toas("Hello");

Vibration(int time) - вызывает вибрацию на устройстве игрока. Имеет атрибут типа int, отвечаещего за продолжительность вибрации (В мил.сек.)
AndroidAPI.Vibration(500);

SetVolumeMusic(int value) - Устанавливает громкость музыки на телефоне. Имеет атрибут типа int, отвечаещего за громкость
AndroidAPI.SetVolumeMusic(10);

StartApp(string packages) - Открывает сторонее приложение. Имеет атрибут типа string, отвечаещего за Package ID
AndroidAPI.StartApp(com.example.app);

ToShare(string message) - метод, с помощь которого можно отправить текст в различные соц. сети. Принимает атрибуты типа string, отвечающие за отправляемое сообщение
AndroidAPI.ToShare("Goog game, bro! Let's go playing!");

********************************
**Разрешения**

PermOnCallPhoneo() - получает разрешение на использование звонков
PermOnRecordAudio() - получает разрешение на записывания аудио
PermOnReadContacts() - получает разрешение на чтение контактов
PermOnRead_Calender() - получает разрешение на чтения календаря(Ивента и тд)
PermOnCamera() - получает разрешение на использование камеры
PermOnWRITE_EXTERNAL_STORAGE() - получает разрешение на записывания файлов(Создание папок, файлов и тд)

*******************************************


**Установка**

Разорхивируйте архив.
Файл AndroidAPILib.aar перенесите по пути Asset -> Plugins -> Android (Если пути нет, то создайте)
Файле AndroidAPI.cs, можете занести в любую папку проекта
