# Mission 2

## Part 0

[Link to video](https://www.youtube.com/watch?v=UUhavvMO2FQ)

## Part1

- Зачем нужен ssh? Ответ на пару предложений.	 
> это протокол, обеспечивающий безопасное удаленное подключение к другим компьютерам. он шифрует данные, что защищает их от перехвата, и позволяет выполнять команды, передавать файлы и управлять серверами с высокой степенью безопасности

- Предположим, у вас есть прямой доступ к серверу(терминалу) под управлением ubuntu. У вас есть коллега Вася, который хочет получить доступ к этому серверу. Он генерирует пару ssh ключей с помощью команды ssh-keygen и дает вам свой публичный ключ. В какой файл на сервере нужно записать ключ, чтобы Вася смог подключиться к терминалу сервера?	 
> в папку .ssh/is_rsa.pub

- Тут вопрос про АПИ. Разберитесь, что такое long polling и webhooks, опишите сами в нескольких предложениях, как они работают.	 
> Long polling — это техника, используемая в веб-разработке для получения обновлений от сервера. при long polling клиент отправляет запрос на сервер и ждет, пока сервер не ответит. если на сервере нет новых данных, он удерживает соединение открытым, пока не появится информация или не истечет таймаут. как только данные становятся доступными, сервер отправляет ответ, и клиент может сразу же отправить новый запрос, чтобы снова ожидать обновлений
Webhooks — это механизм, позволяющий серверу отправлять данные клиенту в режиме реального времени. вместо того чтобы клиент запрашивал данные с определенной периодичностью, сервер инициирует HTTP-запрос к заранее определенному URL на клиенте, когда происходят определенные события (например, изменение данных). это позволяет сократить нагрузку на сервер и уменьшить задержки, так как данные отправляются только при необходимости

- Найдите информацию, что такое issues на гитхабе и для чего нужны. Также вставьте ссылки на пару примеров issues в популярных open source проектах.
> Issues на GitHub — это инструмент для отслеживания задач, ошибок и предложений по улучшению проекта. они позволяют разработчикам и пользователям взаимодействовать, обсуждать проблемы и предлагать изменения 
Issues могут использоваться для:
1. отслеживание ошибок(пользователи могут сообщать о найденных ошибках в коде)
2. запрос функции (участники могут предлагать новые функции или улучшения)
3. обсуждения (Issues могут служить местом для обсуждения различных аспектов проекта, включая архитектуру, дизайн и другие вопросы
4. управление задачами (разработчики могут использовать issues для планирования работы и распределения задач)
примеры: https://github.com/RocketChat/Rocket.Chat/issues
https://github.com/gogs/gogs/issues
https://github.com/Kanaries/Rath/issues

- Ваш проект используется пустую папку images, но гит не поддерживает отслеживание пустых директорий. Что делать?
> создать пустой файл или файл заглушку, например, .gitkeep или .placeholder
