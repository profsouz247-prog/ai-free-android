# Как собрать AI Free APK через GitHub

Этот способ подходит, если компьютер слабый. APK соберётся на серверах GitHub.

## 1. Создай репозиторий

1. Открой https://github.com/
2. Нажми **New repository**
3. Название, например:

```text
ai-free-android
```

4. Выбери **Public** или **Private**
5. Нажми **Create repository**

## 2. Загрузи проект

Самый простой способ:

1. Открой созданный репозиторий
2. Нажми **Add file** → **Upload files**
3. Распакуй архив `ai_free_android_github.zip`
4. Перетащи все файлы и папки в GitHub
5. Нажми **Commit changes**

Важно: загружай содержимое папки проекта, чтобы файл был тут:

```text
.github/workflows/build-apk.yml
```

## 3. Запусти сборку APK

1. Открой вкладку **Actions**
2. Слева выбери **Build AI Free APK**
3. Нажми **Run workflow**
4. Ещё раз **Run workflow**
5. Подожди 5–15 минут

## 4. Скачай APK

1. Открой завершённый workflow
2. Внизу найди **Artifacts**
3. Скачай **AI-Free-APK**
4. Внутри будет:

```text
app-release.apk
```

Это готовое Android-приложение.

## Если сборка не появилась

Проверь, что файл есть именно здесь:

```text
.github/workflows/build-apk.yml
```

## Если GitHub просит включить Actions

Нажми:

```text
I understand my workflows, go ahead and enable them
```
