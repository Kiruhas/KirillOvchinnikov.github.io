# [ИДБ-17-06](https://github.com/stankin/design-part-2/wiki/list-idb-17-06) Овчинников Кирилл

## Курсовой проект по дисциплине "Проектирование информационных систем"

### 1. Определение требований к модели [✋](https://github.com/stankin/design-part-2/wiki/LR-1)

**Тема ВКР:** Разработка и создание модуля “Pick-by-line” для WMS-системы
производственного предприятия

**Объект исследований:** система управления складом

**Предмет исследований:** механизмы использования отдельных складских ячеек для заказов

**Процессы верхнего уровня:** [✋](https://github.com/stankin/design-part-2/wiki/sem1)
* **А1** Управление предприятием
* **А2** Подготовка
* **А3** Производство
* **А4** Складирование
* **А5** Сбыт

**Точка зрения:** Владелец производственного предприятия

**Цель моделирования:** определение процессов, которые можно улучшить

### 2. Функциональное моделирование процессов (IDEF0) [✋](https://github.com/stankin/design-part-2/wiki/LR-1)

#### A-0

![A-0](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A0.png)

#### A0:

![A0](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A1-A5.png)

#### Декомпозиция A1:

![A1](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A1-Dec.png)

#### Декомпозиция A2:

![A2](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A2-Dec.png)

#### Декомпозиция A3:

![A3](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A3-Dec.png)

#### Декомпозиция A4:

![A4](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A4-Dec1.png)

#### Декомпозиция A5:

![A5](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A5-Dec.png)


### 3. Функциональное моделирование программных и информационных средств (DFD) [✋](https://github.com/stankin/design-part-2/wiki/LR-2)

**Конфигурация технических средств:** <рабочие станции, серверы, другое оборудование>

**Конфигурация программных средств:** <одноуровневые, многоуровневые, встроенные, распределенные>

**Допустимые виды хранилищ и их размещение:** <файлы, директории, репозитории, базы данных>

#### Автоматизация процесса A13:

![A13](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A13.png)

#### Автоматизация процесса A21:

![A21](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A21.png)

#### Автоматизация процесса A:

![A23](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A23.png)

#### Автоматизация процесса A:

![A33](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A33.png)

#### Автоматизация процесса A:

![A43](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A43.png)

#### Автоматизация процесса A:

![A51](https://github.com/Kiruhas/KirillOvchinnikov.github.io/blob/master/ramus/A51.png)


### 4. Описание выбранного процесса [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате прецедента (Use Case) [✋](https://github.com/stankin/design-part-2/wiki/LR-4)

Диаграмма UML Use Case
![p4](http://www.plantuml.com/plantuml/proxy?idx=0&src=https://raw.githubusercontent.com/<user/user.github.io/master/<path><file>)

**4.1 Идентификатор прецедента:** ???

**4.2 Название прецедента:** ???

**4.3 Контекст:** ???

**4.4 Участники (actors) и цели (goals):**

| Участник  | Категория  | Цель (goal) |
|---|---|---|
| <роль> | Основной  | <основная цель для роли> |
| <роль> | Внешний  | <основная внешняя цель> |
| <наименование> | Инструмент| <основная функция инструмента> |

**4.5 Предусловия (pre-conditions):**

* <условие наличия потока управления>

* <условие наличия входного потока>

* <условие наличия потока исполнителя>

* <условие наличия потока механизма>

**4.6 Постусловия (post-conditions):**

* <выходной поток>

**4.7 Основной поток выполнения (main flow)**:

| Участник  | Действие (activity)  | Ожидаемый результат |
|---|---|---|
| <роль> | <действие> | <результат с указанием его места размещения> |

**4.8 Исключения (exceptions):**

| Условие (риск) | Последствия | Реакция |
|---|---|---|
| <описание риска> | <описание последствий> | <описание потока сообщений о проблемах> |

**4.9 Альтернативы (alternates):**

| Участник  | Действие (activity)  | Ожидаемый результат |
|---|---|---|
| <роль> | <действие> | <результат с указанием его места размещения> |

**4.10 Временные параметры:**

* **Триггер (событие, стартующее прецедент):** <управляющий поток>

* **Номинальная частота повторения прецедента:** <n раз в смену/сутки/месяц/квартал/год...>

* **Продолжительность прецедента:** <n нормочасов>

### 5. Описание структуры объекта [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате ERD (Class) [✋](https://github.com/stankin/design-part-2/wiki/LR-5)

* **Описываемый объект:** <программа, модуль, сообщение, база данных...>

* **Диаграмма UML Class:**
![p5](http://www.plantuml.com/plantuml/proxy?idx=0&src=https://raw.githubusercontent.com/<user/user.github.io/master/<path><file>)

### 6. Описание алгоритма [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате UML (Sequence) [✋](https://github.com/stankin/design-part-2/wiki/LR-6)

* **Описываемые процессы и потоки данных:** ???

* **Диаграмма UML Sequence:**
![p6](http://www.plantuml.com/plantuml/proxy?idx=0&src=https://raw.githubusercontent.com/<user/user.github.io/master/<path><file>)

### 7. Описание состава [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате UML (Component) [✋](https://github.com/stankin/design-part-2/wiki/LR-7)

* **Описываемый объект:** <комплект поставки>

* **Диаграмма UML Component:**
![p7](http://www.plantuml.com/plantuml/proxy?idx=0&src=https://raw.githubusercontent.com/<user/user.github.io/master/<path><file>)

### 8. Демонстрация реализации (личная страница)

<ссылка или скриншоты>

### 9. Подготовка к интерпретации построенных моделей

**9.1 Используемые паттерны проектирования и разработки [✋](https://github.com/stankin/design-part-2/wiki/sem2):**

* **Процессная модель для сравнения:**

* **Используемые в разработке паттерны и фреймворки:**

**9.2 Используемые паттерны выявления проблем [✋](https://github.com/stankin/design-part-2/wiki/sem3):**
* Муда: <муда>
* Мура: <мура>
* Мури: <мури>

**9.3 Возможные антипаттерны [✋](https://github.com/stankin/design-part-2/wiki/sem4):**

| Категория  | Антипаттерн (риск) | Действие по избежанию |
|---|---|---|
| Разработка | <антипаттерн> | <действие> |
| Архитектура | <антипаттерн> | <действие> |
| Организация | <антипаттерн> | <действие> |
| Среда | <антипаттерн> | <действие> |

### 10. Интерпретация построенных моделей

**10.1 Определение числовых показателей для поставленной цели моделирования:**

**10.2 Определение числовых показателей для цели потенциального проекта автоматизации: [✋](https://github.com/stankin/design-1/wiki/interpret_process)**

**10.3 Расчет потенциального эффекта от автоматизации:**

**10.4 Определение числовых показателей и расчет трудозатрат на разработку программных средств:**

**ВЫВОДЫ**

