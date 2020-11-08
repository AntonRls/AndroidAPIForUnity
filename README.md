# AndroidAPIForUnity
Android API для Unity

В этом репозитории находится плагин для использования Android API в Unity

/* Документация *\

Все методы вызываются через AndroidAPI

Toas(string message) - вызывает всплывающее окно. Имеет атрибут типа string, который отвечает за показываемое сообщение
AndroidAPI.Toas("Hello");

Vibration(int time) - вызывает вибрацию на устройстве игрока. Имеет атрибут типа int, отвечаещего за продолжительность вибрации (В мил.сек.)
AndroidAPI.Vibration(500);

/* Установка *\

Разорхивируйте архив.
Файл AndroidAPILib.aar перенесите по пути Asset -> Plugins -> Android (Если пути нет, то создайте)
Файле AndroidAPI.cs, можете занести в любую папку проекта
