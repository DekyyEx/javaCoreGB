# Используем базовый образ с поддержкой Java
FROM openjdk:8-jdk

# Установка необходимых пакетов
RUN apt-get update && apt-get install -y \
    git \
    maven \
    doxygen \
    graphviz

# Копирование исходных файлов проекта в контейнер
COPY . /app

# Установка рабочей директории
WORKDIR /app


# Формирование документации с помощью Doxygen
RUN doxygen Doxyfile

# Команда по умолчанию, выполняющаяся при запуске контейнера
CMD ["bash"]