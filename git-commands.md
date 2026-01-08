## Основные команды Git

 1. git init

Инициализирует новый репозиторий Git в текущей директории.

**Пример использования**:
```bash
mkdir my-project
cd my-project

git init
```

После выполнения команды в директории будет создана скрытая папка `.git`, которая содержит всю информацию о репозитории.

2. git clone

Клонирует (копирует) существующий репозиторий с удаленного сервера на локальный компьютер.

**Пример использования**:
```bash
git clone https://github.com/username/repository-name.git

git clone https://github.com/username/repository-name.git my-folder

git clone -b branch-name https://github.com/username/repository-name.git
```

3. git add

Добавляет изменения в файлах в область подготовки (staging area) для последующего коммита.

**Пример использования**:
```bash
echo "Hello World" > hello.txt

git add hello.txt

git add .
```

4. git commit

Создает коммит (снимок состояния) с изменениями, которые были добавлены в staging area.

**Пример использования**:
```bash
git commit -m "Добавлен файл README.md"

git commit -m "Добавлен файл README.md

- Добавлена информация о проекте
- Описаны основные функции
- Добавлены инструкции по установке"
```

### 5. git push

Отправляет локальные коммиты в удаленный репозиторий (например, на GitHub).

**Пример использования**:
```bash
git push origin main
```
Перед первым push необходимо настроить удаленный репозиторий:
```bash
git remote add origin <URL-репозитория>
```

### 6. git pull

Загружает изменения из удаленного репозитория и объединяет их с локальной веткой.

**Пример использования**:
```bash
# Получить последние изменения из удаленного репозитория
git pull

# Получить изменения из конкретной ветки
git pull origin main

# Получить изменения без автоматического слияния
git pull --no-merge
```