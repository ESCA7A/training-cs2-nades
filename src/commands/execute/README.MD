# Команды

Директория вызова команд

# Syntax
1. Подгрузка команды: 
> exec training/commands/core/commandName.cfg;

Создание алиаса для дальнейшей работы:
> alias .aliasName .aliasCommandName;

2. Подгрузить в общий конфиг для выполнения:
> Зайти в training/execute/init.cfg
> Заинжектить новый конфиг `exec training/commands/execute/newCommandName.cfg;`