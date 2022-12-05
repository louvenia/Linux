## Part 1. Installation of the OS

**== Task ==**
##### Install **Ubuntu 20.04 Server LTS** without GUI. (Use VirtualBox).
Проверили версию Ubuntu, выполнив команду cat /etc/issue:
![проверка версии Ubuntu 20.04 и команды cat /etc/issue](/src/IMG/%D0%92%D0%B5%D1%80%D1%81%D0%B8%D1%8F%20ubuntu%20%D0%B8%20%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D0%B0.png)

## Part 2. Creating a user

**== Task ==**
Cоздали нового пользователя:
![Cоздали нового пользователя](/src/IMG/%D0%A1%D0%BE%D0%B7%D0%B4%D0%B0%D0%BB%D0%B8%20%D0%BD%D0%BE%D0%B2%D0%BE%D0%B3%D0%BE%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8F.png)
Добавили в группу adm:
![Добавили в группу adm](/src/IMG/%D0%94%D0%BE%D0%B1%D0%B0%D0%B2%D0%B8%D0%BB%D0%B8%20%D0%B2%20%D0%B3%D1%80%D1%83%D0%BF%D0%BF%D1%83%20adm.png)
Проверили командой cat /etc/passwd:
![Проверили командой cat /etc/passwd](/src/IMG/%D0%9F%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%B8%D0%BB%D0%B8%20%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D0%BE%D0%B9%20cat%20%3Aetc%3Apasswd.png)

## Part 3. Setting up the OS network

**== Task ==**
##### Set the machine name as user-1
Установили имя машины как user-1:
![Установили имя машины как user-1](/src/IMG/%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%B8%D0%BB%D0%B8%20%D0%B8%D0%BC%D1%8F%20%D0%BC%D0%B0%D1%88%D0%B8%D0%BD%D1%8B%20%D0%BA%D0%B0%D0%BA%20user-1.png)
Установили имя машины как user-1 в hosts с помощью команды sudo nano /etc/hosts:
![Установили имя машины как user-1 в hosts](/src/IMG/%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%B8%D0%BB%D0%B8%20%D0%B8%D0%BC%D1%8F%20%D0%BC%D0%B0%D1%88%D0%B8%D0%BD%D1%8B%20%D0%BA%D0%B0%D0%BA%20user-1%20%D0%B2%20hosts.png)
Проверка через cat /etc/hosts:
![Проверка через cat /etc/hosts](/src/IMG/%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%B8%D0%BB%D0%B8%20%D0%B8%D0%BC%D1%8F%20%D0%BC%D0%B0%D1%88%D0%B8%D0%BD%D1%8B%20(2).png)
Перезагрузка:
![Перезагрузка](/src/IMG/%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%B8%D0%BB%D0%B8%20%D0%B8%D0%BC%D1%8F%20%D0%BC%D0%B0%D1%88%D0%B8%D0%BD%D1%8B%20(3).png)
##### Set the time zone corresponding to your current location.
Установили часовой пояс, соответствующий текущему местоположению:
![Установили часовой пояс, соответствующий текущему местоположению](/src/IMG/%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%B8%D0%BB%D0%B8%20%D1%87%D0%B0%D1%81%D0%BE%D0%B2%D0%BE%D0%B9%20%D0%BF%D0%BE%D1%8F%D1%81%2C%20%D1%81%D0%BE%D0%BE%D1%82%D0%B2%D0%B5%D1%82%D1%81%D1%82%D0%B2%D1%83%D1%8E%D1%89%D0%B8%D0%B9%20%D1%82%D0%B5%D0%BA%D1%83%D1%89%D0%B5%D0%BC%D1%83%20%D0%BC%D0%B5%D1%81%D1%82%D0%BE%D0%BF%D0%BE%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D1%8E.png)
##### Output the names of the network interfaces using a console command.
Вывели имена сетевых интерфейсов с помощью консольной команды:
![Вывели имена сетевых интерфейсов с помощью консольной команды](/src/IMG/%D0%92%D1%8B%D0%B2%D0%B5%D0%BB%D0%B8%20%D0%B8%D0%BC%D0%B5%D0%BD%D0%B0%20%D1%81%D0%B5%D1%82%D0%B5%D0%B2%D1%8B%D1%85%20%D0%B8%D0%BD%D1%82%D0%B5%D1%80%D1%84%D0%B5%D0%B9%D1%81%D0%BE%D0%B2%20%D1%81%20%D0%BF%D0%BE%D0%BC%D0%BE%D1%89%D1%8C%D1%8E%20%D0%BA%D0%BE%D0%BD%D1%81%D0%BE%D0%BB%D1%8C%D0%BD%D0%BE%D0%B9%20%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B.png)
Пояснение по наличию lo интерфейса: lo (loopback) используется, чтобы компьютер мог обращаться к самому себе и взаимодействовать протоколом динамической конфигурации хоста.
##### Use the console command to get the ip address of the device you are working on from the DHCP server.
Использовали консольную команду, чтобы получить IP-адрес устройства с DHCP-сервера:
![Использовали консольную команду, чтобы получить IP-адрес устройства с DHCP-сервера](/src/IMG/DHCP%20IP.png)
![Использовали консольную команду, чтобы получить IP-адрес устройства с DHCP-сервера](/src/IMG/DHCP%20leases.png)
Расшифруйте DHCP: (Dynamic Host Configuration Protocol) протокол динамического выделения адресов нужен для автоматического получения настройки сервера для компьютеров в сети.
##### Define and display the external ip address of the gateway (ip) and the internal IP address of the gateway, aka default ip address (gw).
Определили и отобразили внешний IP-адрес шлюза (ip) и внутренний IP-адрес шлюза, также известный как IP-адрес по умолчанию (gw):
внутренний IP-адрес шлюза:
![Определили и отобразили внутренний IP-адрес шлюза, также известный как IP-адрес по умолчанию (gw)](/src/IMG/%D0%92%D0%BD%D1%83%D1%82%D1%80%D0%B5%D0%BD%D0%BD%D0%B8%D0%B9%20IP.png)
внешний IP-адрес шлюза (ip):
![Определили и отобразили внешний IP-адрес шлюза (ip)](/src/IMG/%D0%92%D0%BD%D0%B5%D1%88%D0%BD%D0%B8%D0%B9%20IP.png)
##### Set static (manually set, not received from DHCP server) ip, gw, dns settings (use public DNS servers, e.g. 1.1.1.1 or 8.8.8.8).
Установили статические настройки ip, gw, dns:
![Установили статические настройки ip, gw, dns](/src/IMG/%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0%20%D1%81%D1%82%D0%B0%D1%82%D0%B8%D1%81%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D1%85%20%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B5%D0%BA.png)
Проверка статических настроек:
![Проверка статических настроек](/src/IMG/%D0%9F%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%B8%D0%BB%D0%B8%20%D1%81%D1%82%D0%B0%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B5%20%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B8%20ip%2C%20gw%2C%20dns.png)
##### Reboot the virtual machine. Make sure that the static network settings (ip, gw, dns) correspond to those set in the previous point.
Успешно пропинговали удаленные хосты 1.1.1.1 и ya.ru:
![Успешно пропинговали удаленные хосты 1.1.1.1 и ya.ru](/src/IMG/ping.png)

## Part 4. OS Update

**== Task ==**
##### Update the system packages to the latest version
Успешно обновили ОС:
![Успешно обновили ОС](/src/IMG/OS.png)

## Part 5. Using the **sudo** command

**== Task ==**
##### Allow user created in [Part 2](#part-2-creating-a-user) to execute sudo command.
Задаем пароль созданному пользователю user1:
![Задаем пароль созданному пользователю user1](/src/IMG/%D0%97%D0%B0%D0%B4%D0%B0%D0%B5%D0%BC%20%D0%BF%D0%B0%D1%80%D0%BE%D0%BB%D1%8C%20%D1%81%D0%BE%D0%B7%D0%B4%D0%B0%D0%BD%D0%BD%D0%BE%D0%BC%D1%83%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8E.png)
Разрешили пользователю, созданному в части 2 , выполнять команду sudo:
![Разрешили пользователю, созданному в части 2 , выполнять команду sudo](/src/IMG/%D0%A0%D0%B0%D0%B7%D1%80%D0%B5%D1%88%D0%B8%D0%BB%D0%B8%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8E%20%D0%B2%D1%8B%D0%BF%D0%BE%D0%BB%D0%BD%D1%8F%D1%82%D1%8C%20%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D1%83%20sudo.png)
Изменили имя хоста ОС с помощью пользователя, созданного в части 2 (используя sudo):
![Изменили имя хоста ОС с помощью пользователя, созданного в части 2 (используя sudo)](/src/IMG/%D0%97%D0%B0%D1%85%D0%BE%D0%B4%D0%B8%D0%BC%20%D0%B2%20%D0%BD%D0%BE%D0%B2%D0%BE%D0%B3%D0%BE%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8F%20%D0%B8%20%D0%BC%D0%B5%D0%BD%D1%8F%D0%B5%D0%BC%20%D0%B2%20hostname%20%D0%B8%D0%BC%D1%8F%20%D1%85%D0%BE%D1%81%D1%82%D0%B0.png)
Меняем в hosts имя хоста:
Вводим sudo nano /etc/hosts
![Меняем в hosts имя хоста](/src/IMG/%D0%9C%D0%B5%D0%BD%D1%8F%D0%B5%D0%BC%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%20%D1%85%D0%BE%D1%81%D1%82%D0%B0%20%D0%B2%20hosts.png)
Истинное назначение команды sudo: он необходим для строгого ограничения выполнения программ для определенных пользователей с административными привелегиями.
## Part 6. Installing and configuring the time service

**== Task ==**
##### Set up the automatic time synchronisation service.
Вывели время часового пояса и следующей команды NTPSynchronized=yes:
![Вывели время часового пояса и следующей команды NTPSynchronized=yes](/src/IMG/%D0%92%D1%8B%D0%B2%D0%B5%D0%BB%D0%B8%20%D0%B2%D1%80%D0%B5%D0%BC%D1%8F%20%D1%87%D0%B0%D1%81%D0%BE%D0%B2%D0%BE%D0%B3%D0%BE%20%D0%BF%D0%BE%D1%8F%D1%81%D0%B0%20%D0%B8%20%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B%20%D1%81%D0%B8%D0%BD%D1%85%D1%80%D0%BE%D0%BD%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D0%B8.png)

## Part 7. Installing and using text editors

**== Task ==**

##### Install **VIM** text editor (+ any two others if you like **NANO**, **MCEDIT**, **JOE** etc.)
Установили текстовый редактор VIM (+ NANO и JOE):
##### Using each of the three selected editors, create a *test_X.txt* file, where X is the name of the editor in which the file is created. Write your nickname in it, close the file and save the changes.
Используя каждый из трех выбранных редакторов, создали файл test_X.txt , где X — имя редактора, в котором создается файл. Написали в нем свой никнейм, закрыли файл и сохранили изменения:
test_vim.txt for save (:wq - для выхода с сохранением):
![test_vim.txt. Написали в нем свой никнейм, закрыли файл и сохранили изменения](/src/IMG/vim%20nik.png)
test_nano.txt for save (ctrl+x, y - подтверждение сохранения, enter - подтверждение имени файла):
![test_nano.txt. Написали в нем свой никнейм, закрыли файл и сохранили изменения](/src/IMG/nano%20nik.png)
test_joe.txt for save (ctrl+k и q - выход с сохранением):
![test_joe.txt. Написали в нем свой никнейм, закрыли файл и сохранили изменения](/src/IMG/joe%20nik.png)
##### Using each of the three selected editors, open the file for editing, edit the file by replacing the nickname with the "21 School 21" string, close the file without saving the changes.
Используя каждый из трех выбранных редакторов, открыли файл для редактирования, отредактировали файл, заменив никнейм на строку «21 School 21», закрыли файл без сохранения изменений:
test_vim.txt without save (:q! - для выхода бех сохранений):
![test_vim.txt without save (:q!)](/src/IMG/vim%2021%20School%2021.png)
test_nano.txt without save (ctrl+x, n - без сохранения, enter - подтверждение имени файла):
![test_nano.txt without save (ctrl+x, n - подтверждение сохранения, enter - подтверждение имени файла)](/src/IMG/nano%2021%20School%2021.png)
test_joe.txt without save (ctrl+c - выход без сохранения):
![test_joe.txt without save (ctrl+c - выход без сохранения)](/src/IMG/joe%2021%20School%2021.png)
##### Using each of the three selected editors, edit the file again (similar to the previous point) and then master the functions of searching through the contents of a file (a word) and replacing a word with any other one.
Используя каждый из трех выбранных редакторов, снова отредактировали файл (аналогично предыдущему пункту), а затем освоили функции поиска по содержимому файла (слова) и замены слова на любое другое:
test_vim.txt find (Для поиска /, n - для поиска слеующего):
![test_vim.txt find](/src/IMG/vim%20find.png)
test_vim.txt replace (Для замены :%s/louvenia/fruit/g, % - обрабатывать весь файл, q - обработать все найденные строки):
![test_vim.txt replace](/src/IMG/vim%20replace.png)
test_nano.txt find (ctrl+w и ввести то, что нужно найти):
![test_nano.txt find](/src/IMG/nano%20find.png)
test_nano.txt replace (ctrl+\ и ввести то, что нужно найти, нажать клавишу Enter. Затем ввести строку, на которую произвести замену и Enter):
![test_nano.txt replace](/src/IMG/nano%20replace.png)
test_joe.txt find (ctrl+k f - поиск):
![test_joe.txt find](/src/IMG/joe%20find.png)
test_joe.txt replace (в режиме поиска зажать r и ввести замещающее слово):
![test_joe.txt replace](/src/IMG/joe%20replace.png)

## Part 8. Installing and basic setup of the **SSHD** service

**== Task ==**
##### Install the SSHd service.
Установили службу SSHd:
![Установили службу SSHd](/src/IMG/%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%B8%D0%BB%D0%B8%20%D1%81%D0%BB%D1%83%D0%B6%D0%B1%D1%83%20sshd.png)

##### Add an auto-start of the service whenever the system boots.
Добавили автозапуск службы при каждой загрузке системы:
![Добавили автозапуск службы при каждой загрузке системы](/src/IMG/%D0%90%D0%B2%D1%82%D0%BE%D0%B7%D0%B0%D0%BF%D1%83%D1%81%D0%BA%20ssh.png)

##### Reset the SSHd service to port 2022.
Сбросили службу SSHd на порт 2022 (sudo nano sshd_config):
![Сбросили службу SSHd на порт 2022](/src/IMG/Port%202022.png)

##### Show the presence of the sshd process using the ps command. To do this, you need to match the keys to the command.
Показали наличие процесса sshd с помощью команды ps:
![Показали наличие процесса sshd с помощью команды ps](/src/IMG/ps.png)
Значение команды и каждого ключа в ней: это команда для определения работающих в системе программ и оценки используемых ими ресурсов. Выводит статистику. Ключ а - необходим чтобы выбрать все процессы, кроме фоновых, x - опция которая перечисляет все процессы, которые относятся именно к нашей учетной записи,  f - вывести максимум доступных данных, v - показать формат виртуальной памяти, grep - позволяет фильтровать результаты команды.
##### Reboot the system.
Вывод команды netstat -tan:
![Вывод команды netstat -tan](/src/IMG/netstat.png)
Объясните значение ключей -tan, значение каждого выходного столбца, значение 0.0.0.0. в отчете: 
netstat: отображает различные типы сетевых данных в зависимости от выбранного параметра командной строки. -t (--tcp) вывод протокола tcp, -a(--all) список всех портов, -n(--numeric) показать числовые адреса, служебные номера хостов, портов или пользователей.
Прото-протокол (tcp, udp, raw), используемый сокетом.
Recv-Q - количество байтов, не скопированных пользовательской программой, подключенной к этому сокету.
Send-Q — количество байтов, не подтвержденных удаленным хостом.
Локальный адрес — адрес и номер порта локального конца сокета. Если не указан параметр --numeric (-n), адрес сокета преобразуется в его каноническое имя хоста (FQDN), а номер порта преобразуется в соответствующее имя службы.
Внешний адрес — адрес и номер порта удаленного конца сокета. Аналогичен «Локальному адресу».
State - состояние сокета. Поскольку в необработанном режиме нет состояний и обычно состояния не используются в UDP, этот столбец можно оставить пустым.
0.0.0.0 в этом контексте означает, что порт прослушивается на всех «сетевых интерфейсах»
## Part 9. Installing and using the **top**, **htop** utilities

**== Task ==**
##### Install and run the top and htop utilities.
Установите и запустите утилиты top и htop.
Из вывода команды top определили и записали в отчет:
![Из вывода команды top определили и записали в отчет](/src/IMG/top.png)
время безотказной работы: ![время безотказной работы](/src/IMG/%D0%B2%D1%80%D0%B5%D0%BC%D1%8F%20%D0%B1%D0%B5%D0%B7%D0%BE%D1%82%D0%BA%D0%B0%D0%B7%D0%BD%D0%BE%D0%B9%20%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B.png)
количество авторизованных пользователей: ![количество авторизованных пользователей](/src/IMG/%D0%BA%D0%BE%D0%BB%D0%B8%D1%87%D0%B5%D1%81%D1%82%D0%B2%D0%BE%20%D0%B0%D0%B2%D1%82%D0%BE%D1%80%D0%B8%D0%B7%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%BD%D1%8B%D1%85%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D0%B5%D0%B9.png)
общая загрузка системы: ![общая загрузка системы](/src/IMG/%D0%BE%D0%B1%D1%89%D0%B0%D1%8F%20%D0%B7%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B0%20%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D1%8B.png)
общее количество процессов: ![общее количество процессов](/src/IMG/%D0%BE%D0%B1%D1%89%D0%B5%D0%B5%20%D0%BA%D0%BE%D0%BB%D0%B8%D1%87%D0%B5%D1%81%D1%82%D0%B2%D0%BE%20%D0%BF%D1%80%D0%BE%D1%86%D0%B5%D1%81%D1%81%D0%BE%D0%B2.png)
загрузка процессора: ![загрузка процессора](/src/IMG/%D0%B7%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B0%20%D0%BF%D1%80%D0%BE%D1%86%D0%B5%D1%81%D1%81%D0%BE%D1%80%D0%B0.png)
загрузка памяти: ![загрузка памяти](/src/IMG/%D0%B7%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B0%20%D0%BF%D0%B0%D0%BC%D1%8F%D1%82%D0%B8.png)
pid процесса с наибольшим использованием памяти:
![pid процесса с наибольшим использованием памяти](/src/IMG/top%20mem.png)
pid процесса, занимающего больше всего процессорного времени:
![pid процесса, занимающего больше всего процессорного времени](/src/IMG/top%20cpu.png)
Добавьте скриншот вывода команды htop в отчет:
![Добавьте скриншот вывода команды htop в отчет](/src/IMG/htop.png)
отсортировано по PID:
![отсортировано по PID](/src/IMG/pid.png)
PERCENT_CPU:
![PERCENT_CPU](/src/IMG/cpu.png)
PERCENT_MEM:
![PERCENT_MEM](/src/IMG/mem.png)
TIME:
![TIME](/src/IMG/time.png)
отфильтровано для процесса sshd:
![отфильтровано для процесса sshd](/src/IMG/filtr%20sshd.png)
с процессом системного журнала, найденным путем поиска:
![с процессом системного журнала, найденным путем поиска](/src/IMG/filtr%20syslog.png)
с добавленным выводом имени хоста, часов и времени безотказной работы:
![с добавленным выводом имени хоста, часов и времени безотказной работы](/src/IMG/hostname%2C%20clock%2C%20uptime.png)

## Part 10. Using the **fdisk** utility

**== Task ==**

##### Run the fdisk -l command.
Запустили команду fdisk -l:
![Запустили команду fdisk -l](/src/IMG/fdisk.png)
название жесткого диска:![название жесткого диска](/src/IMG/%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%B6%D0%B5%D1%81%D1%82%D0%BA%D0%BE%D0%B3%D0%BE%20%D0%B4%D0%B8%D1%81%D0%BA%D0%B0.png)
его емкость:![его емкость](/src/IMG/%D0%B5%D0%BC%D0%BA%D0%BE%D1%81%D1%82%D1%8C.png)
количество секторов:![количество секторов](/src/IMG/%D0%BA%D0%BE%D0%BB%D0%B8%D1%87%D0%B5%D1%81%D1%82%D0%B2%D0%BE%20%D1%81%D0%B5%D0%BA%D1%82%D0%BE%D1%80%D0%BE%D0%B2.png)
размер подкачки:![размер подкачки](/src/IMG/%D1%80%D0%B0%D0%B7%D0%BC%D0%B5%D1%80%20%D0%BF%D0%BE%D0%B4%D0%BA%D0%B0%D1%87%D0%BA%D0%B8.png)
Отсутствует подкачка

## Part 11. Using the **df** utility

**== Task ==**
##### Run the df command.
Запустили команду df:
![Запустили команду df](/src/IMG/df.png)
Размер раздела:
![Размер раздела](/src/IMG/%D1%80%D0%B0%D0%B7%D0%BC%D0%B5%D1%80%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%20df.png)
используемое пространство:
![используемое пространство](/src/IMG/%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D1%83%D0%B5%D0%BC%D0%BE%D0%B5%20%D0%BF%D1%80%D0%BE%D1%81%D1%82%D1%80%D0%B0%D0%BD%D1%81%D1%82%D0%B2%D0%BE%20df.png)
свободного пространства:
![свободного пространства](/src/IMG/%D1%81%D0%B2%D0%BE%D0%B1%D0%BE%D0%B4%D0%BD%D0%BE%D0%B3%D0%BE%20%D0%BF%D1%80%D0%BE%D1%81%D1%82%D1%80%D0%B0%D0%BD%D1%81%D1%82%D0%B2%D0%B0%20df.png)
процент использования:
![процент использования](/src/IMG/%D0%BF%D1%80%D0%BE%D1%86%D0%B5%D0%BD%D1%82%20%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20df.png)
Определили единицу измерения: 1K-блок (Килобайт)= 1024 байта

##### Run the df -Th command.
Запустили команду df -Th:
![Запустили команду df -Th](/src/IMG/df%20-Th.png)
Размер раздела:
![Размер раздела](/src/IMG/%D1%80%D0%B0%D0%B7%D0%BC%D0%B5%D1%80%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%20df%20-Th.png)
используемое пространство:
![используемое пространство](/src/IMG/%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D1%83%D0%B5%D0%BC%D0%BE%D0%B5%20%D0%BF%D1%80%D0%BE%D1%81%D1%82%D1%80%D0%B0%D0%BD%D1%81%D1%82%D0%B2%D0%BE%20df%20-Th.png)
свободного пространства:
![свободного пространства](/src/IMG/%D1%81%D0%B2%D0%BE%D0%B1%D0%BE%D0%B4%D0%BD%D0%BE%D0%B3%D0%BE%20%D0%BF%D1%80%D0%BE%D1%81%D1%82%D1%80%D0%B0%D0%BD%D1%81%D1%82%D0%B2%D0%B0%20df%20-Th.png)
процент использования:
![процент использования](/src/IMG/%D0%BF%D1%80%D0%BE%D1%86%D0%B5%D0%BD%D1%82%20%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20df%20-Th.png)
Определили тип файловой системы: ext4, 1G = 2 в 30 степени байта

## Part 12. Using the **du** utility


**== Task ==**

##### Run the du command.
Запустили команду du:
![Запустили команду du](/src/IMG/du%20-h.png)
##### Output the size of the /home, /var, /var/log folders (in bytes, in human readable format)
Вывели размер папок /home, /var, /var/log (в байтах, в удобочитаемом формате):
![Вывели размер папок /home, /var, /var/log](/src/IMG/du.png)
##### Output the size of all contents in /var/log (not the total, but each nested element using *)
#Вывели размер всего содержимого в /var/log (не всего, а каждого вложенного элемента, используя *):
![Вывели размер всего содержимого в /var/log](/src/IMG/du%20*.png)

Все через -h и -ha /var/log/*:
![Вывели размер всего содержимого в /home](/src/IMG/duhhome.jpeg)
![Вывели размер всего содержимого в /var](/src/IMG/duhvar.jpeg)
![Вывели размер всего содержимого в /var/log](/src/IMG/duhvarlog.jpeg)
![Вывели размер всего содержимого в /var/log/*](/src/IMG/duhavarlog.jpeg)

## Part 13. Installing and using the **ncdu** utility

**== Task ==**
##### Install the ncdu utility.
Установили утилиту ncdu:
![Вывели размер всего содержимого в /var/log](/src/IMG/ncdu.png)

##### Output the size of the /home, /var, /var/log folders.
Вывели размер папок /home:
![Вывели размер папок /home](/src/IMG/home.png)
Вывели размер папок /var:
![Вывели размер папок /var](/src/IMG/var.png)
Вывели размер папок /var/log:
![Вывели размер папок /var/log](/src/IMG/varlog.png)

## Part 14. Working with system logs

**== Task ==**

##### Open for viewing:
##### 1. /var/log/dmesg
Вывели /var/log/dmesg:
![Вывели /var/log/dmesg](/src/IMG/dmesg.png)
##### 2. /var/log/syslog
Вывели /var/log/syslog:
![Вывели /var/log/syslog](/src/IMG/syslog.png)
##### 3. /var/log/auth.log
Вывели /var/log/auth.log:
![Вывели /var/log/auth.log](/src/IMG/authlog.png)
Записали время последнего успешного входа в систему, имя пользователя и метод входа:
![Записали время последнего успешного входа в систему, имя пользователя и метод входа](/src/IMG/session.png)
Перезапустили службу SSHd:
![Перезапустили службу SSHd](/src/IMG/reboot%20ssh.png)
![Перезапустили службу sshd syslog](/src/IMG/sshsyslog.jpeg)
![Перезапустили службу sshd syslog2](/src/IMG/syslogsshwithoutgrep.jpeg)
![Перезапустили службу sshd status](/src/IMG/sshstatusf.jpeg)

## Part 15. Using the **CRON** job scheduler

**== Task ==**
##### Using the job scheduler, run the uptime command in every 2 minutes.
С помощью планировщика заданий запускали команду uptime каждые 2 минуты:
![С помощью планировщика заданий запускали команду uptime каждые 2 минуты](/src/IMG/crontab.png)
Нашли строки в системных журналах (не менее двух за заданный период времени) о выполнении:
![Нашли строки в системных журналах (не менее двух за заданный период времени) о выполнении](/src/IMG/%20crontab%20syslog.jpeg)

##### Remove all tasks from the job scheduler.
Удалили все задачи из планировщика заданий:
![Удалили все задачи из планировщика заданий](/src/IMG/del%20crontab.jpeg)
