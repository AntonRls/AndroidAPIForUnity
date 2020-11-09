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

ToShare(string message) - Метод, с помощь которого можно отправить текст в различные соц. сети. Принимает атрибуты типа string, отвечающие за отправляемое сообщение
AndroidAPI.ToShare("Goog game, bro! Let's go playing!");

SetBluetooth(bool active) - Метод, позволяющий взаимодействовать с Bluetooth пользователя. Имеет атрибуты типа bool, обозначающие включен ли Bluetooth
AndroidAPI.SetBluetooth(true);

SetLantern(bool act) - Метод, позволяющий взаимодействовать с фонариком пользователя. Имеет атрибуты типа bool, обозначающие включен ли фонарик
AndroidAPI.SetLantern(false);

getAppInstall(string app) - Возвращает, переменную типа bool, которая обозночает установлено ли приложение на устройстве пользователя(true - установлено, false - не установлено). Принимает атрибуты типа string, отвечающего за Package ID
bool app = AndroidAPI.getAppInstall("com.example.app");
if(app) AndroidAPI.Toas("install");
if(!app) AndroidAPI.Toas("don't install");

********************************
**Разрешения**

PermOnCallPhoneo() - получает разрешение на использование звонков

PermOnRecordAudio() - получает разрешение на записывания аудио

PermOnReadContacts() - получает разрешение на чтение контактов

PermOnRead_Calender() - получает разрешение на чтения календаря(Ивенты и тд)

PermOnCamera() - получает разрешение на использование камеры

PermOnWRITE_EXTERNAL_STORAGE() - получает разрешение на записывания файлов(Создание папок, файлов и тд)

********************************************


**Установка**

Разорхивируйте архив.
Файл AndroidAPILib.aar перенесите по пути Asset -> Plugins -> Android (Если пути нет, то создайте)
Файле AndroidAPI.cs, можете занести в любую папку проекта
