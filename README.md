<img align="center" src="images/Pages_Indexing_in_Progress__1.png" alt="Приложение «PrettySearchEngine» в процессе работы">

<h1 align="center">PrettySearchEngine</h1>
<h3 align="center">Локальный поисковый движок, позволяющий индексировать веб-сайты</h3>
<div align="center">&nbsp;</div>

![Static Badge](https://img.shields.io/badge/:PRETTY_SEARCH_ENGINE-SITE_SEARCH-blue)
![Static Badge](https://img.shields.io/badge/:HOW%20TO%20START%20USING-8A2BE2)

![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Portfolio](https://img.shields.io/badge/Portfolio-%23000000.svg?style=for-the-badge&logo=firefox&logoColor=#FF7139)

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Apache Maven](https://img.shields.io/badge/Apache%20Maven-C71A36?style=for-the-badge&logo=Apache%20Maven&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)

### Возможности:
* Парсинг и индексирование страниц веб-сайтов
* Извлечение лемм (lemma, ключ — начальная, словарная форма слова) из проиндексированных веб-страниц
* Подсчёт вхождений найденных лемм
* Сохранение информации о найденных леммах в базе данных MySQL
* Создание сниппетов (фрагментов исходного текста веб-страниц) для последующего их отображения при поиске по базе данных
* Поиск ключей-лемм по базе данных и отображение веб-страниц, в тексте которых встречаются соответствующие им слова в разных формах

### Стек технологий:
* Java 17
* Apache Maven 3.9.2
* Hibernate ORM 6.2
* Spring Boot 2.7.1
* JSOUP 1.15.4
* Lombok 1.18.24
* Apache Lucene 1.5
* MySQL 8.0.33

### Инструкция по развёртыванию приложения:
* Установите Apache Maven
* Установите сервер MySQL
* Создайте базу данных `search_engine`
* Введите веб-адреса и названия сайтов для индексации в следующей секции файла `application.yaml`

![Application_yaml__Configuration__1.png](images/Application_yaml__Configuration__1.png)

* Укажите пользователя и соответствующий ему пароль доступа для соединения с базой данных в этой секции файла `application.yaml`

![Application_yaml__Configuration__1.png](images/Application_yaml__Configuration__2.png)

### Использование приложения:
* Запустите индексацию веб-сайтов
```java
⏵ Run 'Application'
```
* Откройте в веб-браузере страницу http://localhost:8080
* Дождитесь, пока указанные Вами сайты проиндексируются (в зависимости от количества веб-страниц на них, индексация может занять продолжительное время)
* Осуществите поиск ключей-лемм по сформированной в результате индексации базе данных

### Управление приложением:
* Нажатием на кнопку `START INDEXING` запускается индексация веб-сайтов, адреса которых указаны в файле `application.yaml`
* Чтобы остановить индексацию, не дожидаясь её окончания, нажмите на кнопку `STOP INDEXING`
* Кнопкой `ADD/UPDATE` запускается обновление индекса для введённой в поле `Add/update page` страницы веб-сайта (должен быть указан в файле `application.yaml`)

### Скриншоты примеров использования:
* Приложение в процессе индексации

![Application_yaml__Configuration__1.png](images/Pages_Indexing_in_Progress__2.png)

* Индексация веб-страниц завершена

![Application_yaml__Configuration__1.png](images/Pages_Indexing_Done__1.png)
![Application_yaml__Configuration__1.png](images/Pages_Indexing_Done__2.png)
![Application_yaml__Configuration__1.png](images/Pages_Indexing_Done__3.png)

* Поиск вхождений по базе индекса:

![Application_yaml__Configuration__1.png](images/Search_in_Index__Example__1.png)
![Application_yaml__Configuration__1.png](images/Search_in_Index__Example__2.png)

