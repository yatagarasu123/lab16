### Лабораторна робота №16: Advanced TODO List

#### Мета роботи:
Ознайомлення з розширеним управлінням завданнями в Python за допомогою класів і методів.

#### Очікуваний результат:
Набуття практичних навичок у створенні класів, методів і роботи з розкладом завдань.

#### Опис завдання:
Ця лабораторна робота передбачає створення класу Task і Schedule з відповідними методами для управління списком завдань.

#### Виконання роботи:

#### Структура проекту:
Код розділений на класи Task і Schedule. Кожен клас відповідає за різні аспекти управління завданнями і розкладом.

#### Опис файлів:
- **student_main.py**: містить класи Task і Schedule з методами для додавання, видалення, оновлення та управління завданнями.
- **README.md**: описує структуру проекту, опис кожного класу, основні методи з поясненням їх роботи.

#### Опис основних функцій та методів з поясненням їх роботи:

1. **Task Class**:
   - **\_\_init\_\_()**: Ініціалізує об'єкт завдання з параметрами: title, description, due_date, status, priority, notes, recurrence, dependencies.
   - **is_due_today()**: Перевіряє, чи завдання має бути виконане сьогодні. Повертає булеве значення.
   - **\_\_str\_\_()**: Представлення об'єкта завдання у вигляді рядка.

   ```python
   task = Task(title="Buy groceries", description="Milk, Bread, Eggs", due_date=date.today())
   task.is_due_today() 
   ```

2. **Schedule Class**:
   - **\_\_init\_\_()**: Ініціалізує об'єкт розкладу з порожнім списком завдань.
   - **add_task(task: Task)**: Додає завдання до розкладу.
   - **remove_task(task_title: str)**: Видаляє завдання за назвою.
   - **get_task(task_title: str) -> Task**: Повертає об'єкт завдання за назвою.
   - **list_overdue_tasks()**: Повертає список завдань, які прострочені на даний момент.
   - **list_tasks_due_today()**: Повертає список завдань, які мають бути виконані сьогодні.
   - **sort_tasks_by_due_date()**: Повертає список завдань, відсортованих за датою виконання.

   ```python
   schedule = Schedule()
   task = Task(title="Buy groceries", description="Milk, Bread, Eggs", due_date=date.today())
   schedule.add_task(task)
   schedule.get_task("Buy groceries")
   ```

3. **task1: Create Task Class**:
   - Створює клас Task з атрибутами: title, description, due_date, status, priority, notes, recurrence, dependencies.

4. **task2: Add Method to Task Class**:
   - Додає метод is_due_today() до класу Task для перевірки чи завдання має бути виконане сьогодні.

5. **task3: Create Schedule Class**:
   - Створює клас Schedule з методами для управління списком завдань, включаючи додавання, видалення, отримання завдань, виведення прострочених та завдань на сьогодні, сортування за датою виконання.

#### Результати:
Кожен рядок виводить результат виконання відповідної функції, наприклад: 1 рядок - task1, 2 рядок - task2 і так далі.
![image](https://github.com/yatagarasu123/lab16/assets/145234911/4b239805-8db9-4573-bc54-0ffb1caa290c)
![image](https://github.com/yatagarasu123/lab16/assets/145234911/824b22e6-9fd3-4ac9-8340-68f75930b415)


#### Висновки:
Ця лабораторна робота дозволила поглибити розуміння роботи з класами та методами в Python, а також навичок управління завданнями за допомогою розкладу. Застосування класів Task і Schedule дозволяє ефективно організувати і керувати списком завдань, зберігаючи всю необхідну інформацію і забезпечуючи зручний доступ до неї.

#### Інструкції з запуску:
Потрібно відкрити файл student_main.py будь-яким зручним вам способом, де міститься код з класами Task і Schedule, а також README.md, де детально описана структура проекту і функціональність кожного класу. Після запуску програми відповідно до описаних функцій в README.md будуть виведені необхідні результати роботи програми.
