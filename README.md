# Lab_linux
Задание 1 Сервис управления файловым пространством swap

Разработать сервис, который выполняет мониторинг состояния файла подкачки каждые 30 секунд. Если swap заполнен более чем наполовину, создаёт ещё один swap-файл, который удваивает существующее пространство swap.

#Общие требования
##Каждый разработанный сервис должен удовлетворять следующим требованиям:

Сервис должен работать в режиме системной службы, т.е. существовать как системный процесс.
Сервис должен вести собственный журнал событий: событие старта, завершения и обработки сигнала.
Сервис должен выполнять задачу периодически (период написан в задании), обрабатывать сигнал USR1 (выполнять ту же задачу при получении сигнала), а также записывать в журнал подробную информацию по факту выполнения задачи.
Для сервиса должен быть разработан systemd-юнит, которым можно управлять с помощью команды systemctl.
Для сервиса должен быть разработана man-страница с документацией.
Для сервиса должна быть написан модуль безопасности SELinux. Сервис должен работать в собственном домене SELinux имя_сервиса_t.
Сервис должен компилироваться с помощью команды rpmbuild и формировать RPM-пакет, в который будет включён сам сервис, его политика безопасности SELinux, systemd-юнит и man-страница с описанием.
Готовый RPM-пакет должен быть подписан приватным ключом разработчика.
Нужно создать репозиторий (например, локальный), в котором будет находиться RPM-пакет и публичный ключ разработчика. Репозиторий должен быть подключён к системе.
В пакет для каждого сервиса должен быть включён сценарий автоматического тестирования, который выполняет проверку работоспособности сервиса и выводит результат проверки.

#TEAM_WORK
1. Mai Tan Phuoc
2. Ha Phuong Thao
3. Temireeva Najerke
