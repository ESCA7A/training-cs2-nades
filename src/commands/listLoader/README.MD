# Загрузка списков

При появлении новой команды для нее должен быть создан список алиасов для ее исполнения
Допустим, я придумал команду "прыгнуть"
1. Создаю команду в training/commands/core/jumpCmd.cfg
2. Создаю для нее выполняемый конфиг в training/execute/jump.cfg
3. Создаю список всех коротких и длинных алиасов в training/list/core/jumpList.cfg:
```
#filename training/list/core/jumpList.cfg

echoln ".jump       - прыжок."
echoln ".longJump   - длинный прыжок."
```
4. Прокидываю список в training/listLoader/jumpList.cfg:
```
#filename training/listLoader/jumpList.cfg

alias .jumpList "exec training/listLoader/jumpList.cfg";
```
5. Добавляю в training/listLoader/init.cfg - содержит все списки. Прогружается при выполнении сценария `.commands`