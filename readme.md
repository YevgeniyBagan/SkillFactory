# Git и GitHub  
LICENSE:[MIT](license.md)


![logo](https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png)

Git Logo by [Jason Long](https://twitter.com/jasonlong) is licensed under the [Creative Commons Attribution 3.0 Unported License](https://creativecommons.org/licenses/by/3.0/).
____
## **Начнем?**
Что такое **Git** и что такое **Github**

[**Git**](https://ru.wikipedia.org/wiki/Git) (*читается как* «гит») — это система контроля версий файлов для совместной работы над проектами.  
 
[**GitHub**](https://ru.wikipedia.org/wiki/GitHub) — сервис который *хранит*  ваши проекты.  

>Просто хранит? Как облоко ? 

Ну почти, GitHub позволяет осуществлять доступ вашему проекту в реальном времени вам и синхронизировать работу вашей команды(редактировать, удалять и добавлять новые файлы в каком либо из проектов).  
+ Место для хранения одного опеределенного проекта называеться **репозиторий**  

Скачать и установить Git вы можете бесплатно с [официального сайта](https://git-scm.com/downloads)    

### **Пробежимся по основным командам**   
 + `git config` связан с набором команд позволяющий настраивать конфигурации и парамерты
    + `git config --global user.name` — Показывает имя пользователя
    + `git config --global user.name` 'new user' — Изменяет имя пользователя
    + `git config --global user.email` — Показывает email пользователя
    + `git config --global user.email` 'test@mail.ru' — Изменяет email пользователя

 + `git init`
позволяет проинициализировать репозиторий в текущей папке


+  `git commit` — это операция, которая берет все подготовленные изменения и отправляет их 
  в репозиторий как единое целое. Другими словами  делает снимок состояния проекта на текущий момент времени  
    + `git commit -m "текст сообщения"` — создаcт коммит с сообщением  
  + `git status` показывает текущий статус
+ `git add` добавить отслеживание файла   
  
 ```php
    git add index.html  добавит отслеживание файла "index.html"
 ```
  + `git add .` добавит все текущие файлы
+ `git push` заливает текущие локальные коммиты в удаленный репозиторий 
+ `git pull` забирает изменения с удаленного репозитория в локальный
+ `git clone` клонирует проект с удаленного репозитория


## **Ветвление(branch).** 
Ветвление  одновременно и сложная и простая тема, поэтому мы рассмотрим её (как и команды связанные с ней) отдельно.   
 Ветвление позволяет создавать паралельные пути разработки от основной линии  и продолжаеть работу, не вмешиваясь в основную линию.
 >Что это дает? И зачем нужно?

*Вы любите пирожки?* (~~я нет~~)  
 Представим что у вас пекарня, вы начинали в одиночку и справлялись с процессом производста пирогов самостоятельно, держали весь процес и рецепты в голове . Пироги стали пользоваться спросом и вам пришлось расширяться набирая новых сотрудников, раздавая каждому по полномочиям в зависимости от их навыков. Так же умеет и Git , разграничивать доступ к определенным файлам на общей кухне(в репозитории), в окнце концов мы же не хотим что бы уборщик месил тесто. Никакого пренибрежения, но каждый должен заниматься своим профилем работы . 

 Раньше вы изготавливали пирожки только капустой и процесс их изготовления был вполне линейный, вы знаете сколько класть ингридиентов , процесс полностью налажен, проверен временем и потребителями , но теперь отдел маркетинга предложил вам  расширить ассортимент и использовать в качестве начинки  малиновое варенье . Но вы не готовы сразу пускать новые пирожки в производство, вам не известно как поведет себя новая начинка со "старым"
тестом, для этого и нужно **ветвление**. Вы всегда можете создать экспирементальну(новую) линию(паралельную) производства отдельно от основной (*main/master*) ветки для проверок и устранение неполадок перед тем как позволить пользоваться прокудтом потребителю. После того как процесс налажен и провен вы всего можете обьединить(*merge*) уже испраные линии производства. И это лишь малая толика всех возможностей работы с ветвлением.

### **Команды для работы с ветками**

 + `git branch` — показывает список веток  
    + `git branch "имя  ветки"` — создает новую ветку 
    + `git branch -D "имя ветки"` — удаляет ветку
+ `git checkout` переключение между ветками
  + `git checkout "имя ветки"` — переключается на последний коммит в ветке
  + `git checkout -b "имя ветки"` — создает и переключается на ветку
+ `git merge` cовмещает текущую ветку с указанной   
  + `git merge "имя ветки"` — совмещает текущую ветку с указанной в кавычках


_____


*При создании данной инструкции использовалась информации из данных источников*  
- [x] [Видео](https://www.youtube.com/watch?v=zZBiln_2FhM&t=1382s)   
- [x] [Текст](https://git-scm.com/book/ru/v2/%D0%92%D0%B5%D1%82%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D0%B2-Git-%D0%9E-%D0%B2%D0%B5%D1%82%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B8-%D0%B2-%D0%B4%D0%B2%D1%83%D1%85-%D1%81%D0%BB%D0%BE%D0%B2%D0%B0%D1%85)  


