# Forge AdminTools

## Команды

### Управление игроками

| Команда | Разрешение | Описание | Синтаксис | Алиасы |
|---------|------------|----------|-----------|--------|
| `back` | `forge.back` | Возвращает игрока на место смерти | `/back` | `tpdeath` |
| `checkhealth` | `forge.checkhealth` | Проверяет уровень здоровья указанного игрока | `/checkhealth [игрок]` | `chhealth`, `hp` |
| `checkstats` | `forge.checkstats` | Отображает текущую статистику игрока | `/checkstats [игрок]` | `chstats`, `stats` |
| `clearinventory` | `forge.clearinventory` | Очищает инвентарь игрока полностью или по категориям | `/clearinventory [игрок] [категория]` | `ci`, `clearinv`, `invclr` |
| `dropallitems` | `forge.dropallitems` | Выбрасывает все предметы из инвентаря игрока | `/dropallitems [игрок] [-включая_экипировку]` | `dropitems`, `ditems` |
| `dropweapon` | `forge.dropweapon` | Заставляет игрока выбросить его оружие | `/dropweapon <игрок>` | `drwep`, `dwep`, `dropgun` |
| `forcerespawn` | `forge.forcerespawn` | Принудительно возрождает игрока | `/forcerespawn <игрок> [home/bed/random]` | `respawn`, `forceresp` |
| `freeze` | `forge.freeze` | Замораживает или размораживает игрока | `/freeze <игрок> [время]` | `frz`, `hold` |
| `mute` | `forge.mute` | Отключает возможность чата для игрока на определенное время | `/mute <игрок> <время> [причина] \| /mute check <игрок>` | `muteplayer`, `silence` |
| `unmute` | `forge.unmute` | Снимает мут с игрока | `/unmute <игрок> [причина]` | `unmuteплayer`, `unsilence` |
| `restorestats` | `forge.restorestats` | Полностью восстанавливает характеристики игрока | `/restorestats` | - |

### Управление экономикой и навыками

| Команда | Разрешение | Описание | Синтаксис | Алиасы |
|---------|------------|----------|-----------|--------|
| `experience` | `forge.experience` | Выдаёт, устанавливает или отнимает опыт у игрока | `/experience <+/-/=количество> [игрок]` | `exp`, `xp` |
| `maxskills` | `forge.maxskills` | Максимально прокачивает все навыки игрока | `/maxskills [игрок] [группа]` | `ms`, `skills`, `skillmax` |
| `reputation` | `forge.reputation` | Изменяет репутацию игрока | `/reputation [+/-/=]<количество> [игрок]` | `rep` |

### Управление объектами и миром

| Команда | Разрешение | Описание | Синтаксис | Алиасы |
|---------|------------|----------|-----------|--------|
| `attachment` | `forge.attachment` | Устанавливает или снимает обвесы на оружие игрока | `/attachment [ID обвеса или 'remove' тип или 'info']` | `att`, `setattachment` |
| `clearitems` | `forge.clearitems` | Удаляет все предметы в указанном радиусе или на всей карте | `/clearitems [радиус]` | `removeitems`, `ritems` |
| `destroy` | `forge.destroy` | Удаляет баррикады, строения или транспорт | `/destroy [радиус] [тип: all/barricade/structure/vehicle] [опции: -confirm/-owner <steamid>/-id <itemid>]` | `des` |
| `info` | `forge.info` | Показывает информацию о баррикаде, структуре или транспорте | `/info` | `whois`, `getinfo` |
| `refuel` | `forge.refuel` | Заправляет транспорт или генераторы | `/refuel [радиус]` | - |
| `repair` | `forge.repair` | Чинит баррикады, строения или транспорт | `/repair [радиус]` | - |
| `restart` | `forge.restart` | Перезапускает сервер с таймером и сохранением мира | `/restart <время в секундах>` | - |

### Особые возможности

| Команда | Разрешение | Описание | Синтаксис | Алиасы |
|---------|------------|----------|-----------|--------|
| `jump` | `forge.jump` | Активирует или деактивирует режим Jump | `/jump` | `j` |
| `speedjump` | `forge.speedjump` | Изменяет скорость бега и силу прыжка | `/speedjump [скорость] [прыжок] или reset` | `sjump` |

## Дополнительные разрешения

| Разрешение | Описание |
|------------|----------|
| `forge.clearinventory.other` | Возможность очищать инвентарь других игроков |
| `forge.experience.other` | Возможность изменять опыт других игроков |
| `forge.reputation.other` | Возможность изменять репутацию других игроков |
| `forge.mute.admin` | Возможность мутить администраторов |
| `forge.mute.permanent` | Возможность давать постоянный мут |
| `forge.mute.extended` | Возможность давать мут длительностью более 30 дней |
| `forge.mute.override` | Возможность менять мут, выданный другим админом |
| `forge.unmute.others` | Возможность снимать мут, выданный другими админами |
| `forge.unmute.permanent` | Возможность снимать постоянный мут |

## Настройка вебхуков Discord

Плагин поддерживает отправку уведомлений о действиях администраторов в Discord через вебхуки. Для настройки укажите URL вебхука в файле конфигурации.
