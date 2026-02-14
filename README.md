# Инструкция по добавлению бризера Tion Bio X в Home Assistant

- Установить HACS, если он не установлен [HACS](https://hacs.xyz/);
- Добавить в Home Assistant интеграцию [LocalTuya integration](https://github.com/rospogrigio/localtuya/) (не путать с Tuya Local!);
- По инструкции из [README](https://github.com/rospogrigio/localtuya/blob/master/README.md) localtuya добавляем интеграцию и связываем HA с аккаунтом на платформе разработчика;


```markdown
| ID  | Friendly Name           | Platform   | Device Class | Minimum Value | Maximum Value | Valid Entries                      | User Friendly Options                     |
|-----|-------------------------|------------|--------------|---------------|---------------|------------------------------------|-------------------------------------------|
| 101 | Питание        		 | switch     | -            | -             | -             |                                    |                                           |
| 102 | Скорость вентилятора    | number     | -            | 0             | 7             |                                    |                                           |
| 103 | Звук                	| switch     | -            | -             | -             |                                    |                                           |
| 104 | Световая индикация      | select     | -            | -             | -             | 0;50;100                           | 0%;50%;100%                               |
| 108 | Подогрев воздуха   	 | number     | -            | 0             | 30            |                                    |                                           |
| 112 | Температура снаружи     | sensor     | temperature  | -             | -             |                                    |                                           |
| 115 | Ресурс фильтра          | sensor     | enum         | -             | -             | color0;color1;color2;color3;color4 |                                           |
| 133 | Цвет панели             | select     | -            | -             | -             |                                    | Бирюзовый;Фиолетовый;Зелёный;Белый;Желтый | 
```

*Версия LocalTuya integration: 5.2.3
