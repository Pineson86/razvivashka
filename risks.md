# План управления и оценки рисков

## 1. Идентификация потенциальных рисков проекта

| Риск                           | Описание | Вероятность | Влияние | Уровень риска |
|--------------------------------|-----------------------------------------------------------|----------------|------------|--------------|
| **Задержки в разработке**     | Непредвиденные технические сложности или недостаток ресурсов могут замедлить разработку. | Средняя (50%) | Высокое | Высокий |
| **Низкое качество контента**  | Обучающие материалы могут не соответствовать педагогическим стандартам или ожиданиям детей. | Низкая (30%) | Среднее | Средний |
| **Превышение бюджета**        | Непредвиденные расходы на оборудование, рекламу или зарплаты могут превысить плановый бюджет. | Средняя (40%) | Высокое | Высокий |
| **Низкий интерес аудитории**  | Целевая аудитория (дети, родители, педагоги) может не проявить ожидаемого интереса к приложению. | Средняя (50%) | Высокое | Высокий |
| **Технические сбои**          | Ошибки в коде, проблемы с сервером или совместимостью могут нарушить работу приложения. | Средняя (40%) | Среднее | Средний |
| **Утечка данных пользователей** | Нарушение безопасности может привести к компрометации данных детей и родителей. | Низкая (20%) | Критическое | Высокий |
| **Изменение требований законодательства** | Новые законы о защите данных детей или образовательных стандартах могут потребовать доработок. | Низкая (30%) | Среднее | Средний |

### Вероятность:
- Низкая (<30%)  
- Средняя (30-50%)  
- Высокая (>50%)  

### Влияние:
- Низкое (минимальные последствия)  
- Среднее (затрагивает сроки/бюджет)  
- Высокое (угрожает успеху проекта)  
- Критическое (остановка проекта)  

### Уровень риска:
- Низкий (низкая вероятность и влияние)  
- Средний (смешанные показатели)  
- Высокий (высокая вероятность и/или влияние)  

---

## 2. Стратегии и планы управления рисками

### 2.1 Задержки в разработке  
**Стратегия:** Проактивное планирование и мониторинг.  
**План смягчения:**  
- Использовать Agile-методологию с двухнедельными спринтами для раннего выявления проблем.  
- Назначить резервное время (2 недели) в графике на каждом этапе разработки.  
- Привлечь дополнительного разработчика (Middle) на этапе технической разработки, если сроки начнут срываться.  

**План реагирования:**  
- Перераспределить задачи между Backend и Frontend-разработчиками для ускорения работы.  
- Сократить объем необязательных функций (например, сложные анимации) в пользу базового функционала.  

### 2.2 Низкое качество контента  
**Стратегия:** Контроль качества на ранних этапах.  
**План смягчения:**  
- Проводить регулярные проверки контента педагогом-консультантом на этапе разработки (каждые 2 недели).  
- Организовать фокус-группу из 5-10 детей и родителей для тестирования материалов до финального релиза.  

**План реагирования:**  
- Переработать проблемные материалы с привлечением дополнительного контент-райтера в течение 1 месяца.  
- Выпустить обновление приложения с исправленным контентом после обратной связи от пользователей.  

### 2.3 Превышение бюджета  
**Стратегия:** Финансовый контроль и резервирование.  
**План смягчения:**  
- Включить резервный фонд в **400,000 RUB** (10% от бюджета) для покрытия непредвиденных расходов.  
- Ежемесячно отслеживать расходы и сравнивать с плановым бюджетом.  

**План реагирования:**  
- Сократить затраты на рекламу (например, с **171,000 RUB** до **100,000 RUB**) в пользу органического продвижения.  
- Пересмотреть контракты с подрядчиками для снижения ставок на 10-15%.  

### 2.4 Низкий интерес аудитории  
**Стратегия:** Активное продвижение и адаптация.  
**План смягчения:**  
- Провести предварительную рекламную кампанию за 2 месяца до релиза с бюджетом **50,000 RUB** для тестирования интереса.  
- Разработать демо-версию приложения для бесплатного доступа на 7 дней.  

**План реагирования:**  
- Добавить популярные темы (например, персонажей из мультфильмов) в контент на основе обратной связи.  
- Увеличить бюджет на рекламу в социальных сетях на **20%** для привлечения новых пользователей.  

### 2.5 Технические сбои  
**Стратегия:** Тестирование и резервирование.  
**План смягчения:**  
- Провести стресс-тестирование приложения на **10,000 пользователей** перед релизом.  
- Настроить автоматическое резервное копирование данных каждые 24 часа на сервере AWS.  

**План реагирования:**  
- Организовать команду быстрого реагирования (Backend и Frontend-разработчики) для исправления сбоев в течение **12 часов**.  
- Выпустить патч с исправлениями в течение **48 часов** после обнаружения проблемы.  

### 2.6 Утечка данных пользователей  
**Стратегия:** Усиление безопасности.  
**План смягчения:**  
- Использовать **AES-256** для шифрования данных и **bcrypt** для паролей с самого начала разработки.  
- Провести аудит безопасности сторонним специалистом перед релизом (**50,000 RUB**).  

**План реагирования:**  
- Немедленно уведомить пользователей об утечке и сбросить пароли всех аккаунтов.  
- Привлечь эксперта по кибербезопасности для устранения уязвимости в течение **72 часов**.  

### 2.7 Изменение требований законодательства  
**Стратегия:** Мониторинг и гибкость.  
**План смягчения:**  
- Назначить аналитика для ежемесячного мониторинга изменений в законодательстве о данных детей.  
- Разработать модульную архитектуру приложения для быстрой адаптации под новые требования.  

**План реагирования:**  
- Выделить **2 недели** и бюджет **100,000 RUB** на доработку приложения в случае новых требований.  
- Обновить пользовательское соглашение и уведомить пользователей через приложение.  

---

## 3. Итоговый план управления рисками

| Риск | Стратегия | Смягчение | Реагирование | Ответственный |
|------|----------|-----------|--------------|---------------|
| **Задержки в разработке** | Проактивное планирование | Agile, резерв времени, доп. разработчик | Перераспределение задач, сокращение функций | Backend/Frontend-разработчики |
| **Низкое качество контента** | Контроль качества | Проверка педагогом, фокус-группа | Переработка контента, обновление | Контент-райтер |
| **Превышение бюджета** | Финансовый контроль | Резерв 400,000 RUB, мониторинг расходов | Сокращение рекламы, пересмотр контрактов | Аналитик |
| **Низкий интерес аудитории** | Активное продвижение | Предварительная реклама, демо-версия | Добавление тем, увеличение рекламы | Маркетолог |
| **Технические сбои** | Тестирование | Стресс-тестирование, резервное копирование | Быстрое исправление, патч | Backend/Frontend-разработчики |
| **Утечка данных пользователей** | Усиление безопасности | Шифрование, аудит безопасности | Уведомление, устранение уязвимости | Backend-разработчик |
| **Изменение требований законодательства** | Мониторинг | Анализ законодательства, модульная архитектура | Доработка, обновление соглашения | Аналитик |
