# Сборка в Android Studio

Этот раздел описывает, как собрать мобильное приложение «SHISHKA» из исходников в Android Studio.

## Импорт проекта

1. Откройте Android Studio.
2. Выберите **File → Open**.
3. Укажите папку с проектом `shishka-android`.
4. Дождитесь синхронизации Gradle.

![Проект в Android Studio](images/android-studio.png)

## Структура проекта


## Основные зависимости

В файле `app/build.gradle` должны быть указаны:

```gradle
dependencies {
    implementation 'com.squareup.retrofit2:retrofit:2.9.0'
    implementation 'com.squareup.retrofit2:converter-gson:2.9.0'
    implementation 'com.squareup.okhttp3:logging-interceptor:4.9.3'
    implementation 'androidx.appcompat:appcompat:1.6.1'
    implementation 'com.google.android.material:material:1.9.0'
}


