
# 👋 Привет! Я - твой тренировочный конфиг для Counter-Strike

🎯 **Замечательный конфиг, напичканный командами для тренировок**


---

## 📚 Содержание

| № | Глава |
|:---:|:---|
| 1️⃣ | [Введение](#part-1) |
| 2️⃣ | [Получение ножа](#part-2) |
| 3️⃣ | [Очищение карты и перемотка времени](#part-3) |
| 4️⃣ | [Восстановление ХП](#part-4) |
| 5️⃣ | [Боты](#part-5) |
| 6️⃣ | [Бомба](#part-6) |
| 7️⃣ | [Подключение спотов для тренировки](#part-7) |
| 8️⃣ | [Быстрые команды](#part-8) |
| 9️⃣ | [Доступные карты](#part-9) |
| 🔟 | [Ручная установка конфига](#part-10) |
| 1️⃣1️⃣ | [Легкая установка конфига](#part-11) |


---

## <a name="part-1">🎮 PART 1. Введение</a>

**Как я вас встречаю?**

При загрузке конфига расписаны основные методы работы с ним 🎯

<a name="part-start">![exec.png](./../../src/gif/exec.gif)</a>

💡 *Весь процесс взаимодействия происходит через консоль. Не переживай - команды простые, и всегда есть подсказки!*

---

## <a name="part-2">🔪 PART 2. Ножи</a>

**Начнем со всеми любимого - список доступных ножей!**

**Как использовать:**
```
.dropon			# Разрешить дроп ножей
.batterfly-drop		# Создать нож
.dropoff		# Запретить дроп ножей
```

![knifes.gif](./../../src/gif/knifes.gif)

---

## <a name="part-3">⏱️ PART 3. Время и карта</a>

> ❓ *"О, Боже, я миснул смок и теперь ждать 18 секунд..."*

**Решение есть!**

🚀 **`.skiptime`** - ускорить время на сервере (вместо 18 сек → 2 сек)

🧹 **`.clearmap`** - очистить карту моментально (все гранаты ревилятся)

![skiptime_clearmap.gif](./../../src/gif/skiptime_clearmap.gif)
---


## <a name="part-4">❤️ PART 4. Здоровье</a>

> ❓ *"Хочу чекнуть связку хае+молот, но осталось 20ХП..."*

**Решение простое:**

💊 **`.heal`** или **`.hp`** - восстановить 100 HP у всех на сервере

🎯 *Пользуйся и не умирай каждый раз!*

![hp.gif](./../../src/gif/hp.gif)
---

## <a name="part-5">🤖 PART 5. Боты</a>

> ❓ *"Боты крутятся и не слушаются..."*

**Управление ботами:**

📋 **`.botList`** - список команд для ботов

✨ *Боты могут присесть, встать, спавниться и всегда смотрят на тебя!*

![botlist.gif](./../../src/gif/botlist.gif)
---

## <a name="part-6">💣 PART 6. Бомба</a>

> ❓ *"Что можно наворотить с пачкой?"*

**Возможности с бомбой:**

📋 **`.c4List`** - список команд для работы с бомбой

⚡ *Можно выставить таймер, наспавнить бомбу и повзрывать карту*

---

## <a name="part-7">📍 PART 7. Споты для тренировки</a>

> ❓ *"Я сюда за раскидами пришел!"*

**Как использовать споты:**

1. Выбери карту: `.de_anubis`
2. Выбери сторону: `.ct` или `.t`
3. Получи подробные инструкции!

**Пример в консоли:**
```cfg
.de_anubis
[InputService] execing .aliases/training/maps/de_anubis/main.cfg

.ct
[InputService] execing .aliases/training/maps/de_anubis/ct.cfg

.spawn1
[ваша моделька появится на текущей карте de_anubis на спавне для ct с номером 1]
```

![setposes.gif](./../../src/gif/setposes.gif)
---

## <a name="part-8">⚡ PART 8. Быстрые команды</a>

> ❓ *"Забыл команды?"*

**Помощь по командам:**
- **`.commands`** - список всех команд

**Быстрые алиасы:**
```
.clearmap ↔ .ff ↔ .clear    # Очистка карты
.heal     ↔ .hp             # Восстановление ХП
.skiptime ↔ .st ↔ .skip     # Перемотка времени
```

---

## <a name="part-9">🗺️ PART 9. Доступные карты</a>

**Карты с инста гранатами:**

| Карты | Готово к использованию |
|---|---|
| `.de_ancient`		| ✅ |
| `.de_anubis`		| ✅ |
| `.de_dust2`		| ✅ |
| `.de_inferno`		| ✅ |
| `.de_mirage`		| ✅ |
| `.de_nuke`		| ✅ |
| `.de_train`		| ✅ |
| `.de_vertigo`		| ⏳ |
| `.de_cobblestone`	| ⏳ |

---

## <a name="part-10">⚙️ PART 10. Ручная установка</a>

> ❓ *"Как это запустить?"*

**Пошаговая установка:**

1. Перейти в последние релизы <a href="https://github.com/ESCA7A/training-cs2-nades/releases">[клик]<a>
2. скачать архив Source code
3. ПКМ по архиву -> извлечь в текущую папку
4. 📁 Скопируйте извлеченную директорию в папку игры по пути cs:
   ```
   <путь_к_cs2>/csgo/cfg/
   ```

5. 📄 Зайди в папку `training-cs2-nades-Z.X.C/training` Скопируй `example.training.cfg`, перемести в папку /cfg

6. 🔄 В папке cfg переименуй файл `example.training.cfg` -> `training.cfg` 

7. Открой в текстовом редакторе training.cfg и замени пути:

	7.1. `exec training/main.cfg;` -> `exec <training-cs2-nades-Z.X.C>/training/main.cfg;`

	7.2. `exec_async training/helloworld.cfg;` -> `exec_async <training-cs2-nades-Z.X.C>/training/helloworld.cfg;`

8. 🎮 Зайди в игру на любую карту и введи в консоли: `exec training` - [Наглядный запуск в игре](#part-1)


9. 🎉 *Учи гранаты с удовольствием, а главное - бесплатно!*

---

## <a name="part-11">⚙️ PART 11. Easy Installation</a>

> ❓ *"I'm too lazy. How do I run this?"*

**Step-by-step installation:**

1. Go to the latest releases <a href="https://github.com/ESCA7A/training-cs2-nades/releases">[click]<a>
2. Download the Source code archive
3. Right-click the archive -> extract to the current folder
4. 📁 Copy the extracted directory to the game folder along the path cs:
```
<path_to_cs2>/csgo/cfg/
```

5. 🚀 Run cs-nades.exe
<details>
<summary>Learn more about cs-nades.exe</summary>
<a href="https://github.com/ESCA7A/cs2-nades-runner)">Go to source</a>
</details>

6. 🎮 Launch the game on any map and enter `exec training` in the console - [Visual in-game launch](#part-1)

7. 🎉 *Learn grenades with pleasure, and best of all - for free!*

---
