# Paper template
This template is for academic papers. It can be used inside of GitHub, with Obsidian or with Zettlr. Russian below ↓↓↓

## Quick start
1. Click "Use this template" and create a new pository for your paper
2. Open this project folder in your code editor — here on GitHub by clicking `.` or by cloning it to your machine (with command line or with GitHub Desktop)  
3. Make a new file inside of the Text folder. It can a section of a collaborative paper or your entire paper
4. Add a bibliography `.json` file to the `/service` folder
5. Write your paper
6. Send it to the repo via git or GitHub Desktop (if it's on your machine) or just sumbit if you're working inside GitHub. 
7. Get a compiled paper in the repo as "output.pdf" file

Here is a [useful video to get started](https://www.youtube.com/watch?v=J86Pm62XM_Q) — you can install plugins right inside of the GitHub code editor! 

## Как начать работать с шаблоном

### Открываем шаблон
1. Скачайте и установите [GitHub Desktop](https://desktop.github.com/), [Obsidian](https://obsidian.md) и [Zotero](https://zotero.org). Когда Zotero предложит установить Zotero Connector, согласитесь и установите — он понадобится позже.
2. Если у вас нет аккаунта на GitHub, [зарегистрируйтесь](https://github.com/signup).
3. Клонируйте этот репозиторий на свой компьютер с помощью GitHub Desktop — вот [инструкция](https://docs.github.com/ru/desktop/contributing-and-collaborating-using-github-desktop/adding-and-cloning-repositories/cloning-a-repository-from-github-to-github-desktop). А здесь — [вводное видео про Git, GitHub и как и зачем этим пользоваться](https://www.youtube.com/watch?v=8Dd7KRpKeaE).
5. Если в Obsidian у вас нет плагинов вроде Citation и других, то скачайте [папку с дефолтными настройками Obsidian](https://dl.dropboxusercontent.com/s/zvgds9kfhtivp0z/.obsidian.zip) и разархивируйте её в корень проекта.
6. Скачанную папку с этим шаблоном можно использовать как отдельное хранилице Obsidian (это значит, что для каждой статьи — отдельное хранилище), либо как папку внутри существующего хранилища, например, сделать папку Papers. 
7. Откройте Obsidian, выберите **"Open folder as a vault"** (в первом случае), либо найдите и откройте скачанную папку. Вы увидите что-то подобное:
![report-repo-vault.png](service/report-repo-vault.png)

1. Это текстовый редактор, в котором мы будем писать статью, используя язык Markdown. Здесь [короткая справка, как писать на Markdown](https://www.markdownguide.org/basic-syntax/) (там просто, правда).
3. Почитайте шаблон и поэкспериментируйте с ним, пока не разберётесь, как им пользоваться.

### Настраиваем Zotero
1. Если на пользовались рефереренс-менеджерами, то посмотрите [введение](https://www.youtube.com/watch?v=JG7Uq_JFDzE).
2. Создайте в Zotero коллекцию «Моя новая крутая статья», добавьте несколько статей, желательно сразу релевантных вашей теме
4. Установите плагин [Better BibTex](https://retorque.re/zotero-better-bibtex/installation/): скачайте [установочный файл `*.xpi` здесь](https://github.com/retorquere/zotero-better-bibtex/releases/tag/v6.7.94), затем в Zotero перейдите во вкладку «Инструменты» → «Дополнения» → нажмите на шесетёрнку, выберите "Install Add-On from file…" и укажите скачанный xpi-файл.
5. Настройте BetterBibTex. Для этого в Zotero перейдите во вкладку «Инструменты» → "Better BibTex" → "Open Better BibTex Preferences". После этого в поле "Citation Key formula" замените всё написанное на `auth.lower+year` и сохраните изменения.
3. Экспортируйте коллекцию «Моя новая крутая статья» в папку `service` — её можно найти внутри папки с отчётом. Основные шаги: нажать правой кнопкой на коллекцию, выбрать «Экспортировать», в названии файла скопировать название вашего файла из Obsidian (например, `010_shevchenko_epistemic-networks`), выбрать формат CSL-JSON, **нажать чекбокс "Keep Updated"**, а затем "ОК". Если нужно, более детально рассказано [здесь](https://www.youtube.com/watch?v=D9ivU_IKO6M). Хотя в видео экспортируют всю библиотеку Zotero, вам **нужно экспортировать только коллекцию «Отчёт»**.
1. Найдите тестовые статьи и попробуйте вставить их в созданный ранее файл. Это делается с помощью клавиш `Ctrl + Shift + E` — выпадает содержимое папки «Моя новая крутая статья», которую вы создали в Zotero.
![citation-picker.png](service/citation-picker.png)

2. Ещё раз убедитесь, что вы положили свой файл с библиографией в папку `service` (это правда важно).


### Отправляем написанный файл в GitHub
Когда вы закончили работу над текстом, нужно отправить ваш текст в GitHub — там из него и файлов коллег, если вы работаете с кем-то (а так можно) автоматически будет собираться файл статьи в PDF. Как отправить файл:
1. Зайти в GitHub Desktop — там покажутся все изменения, которые вы сделали
3. Нажать "Fetch"
4. Выбрать галками только файлы в папках `text`, `service` и `images` (если вы загрузили библиографию и картинки соответственно). Лишних файлов быть не должно, но это превентивная мера. 
5. Слева внизу в маленьком текстовом поле рядом с вашей аватаркой кратко написать суть ваших изменений, например, «добавил цели и задачи» или «написала про блокмоделинг в разделе методологии». Если хотите, можете написать подробнее в окошке ниже. Там же можно отмечать других участников.
6. Нажать кнопку "Commit"
7. Нажать на кнопку "Push" в том же месте, где вы нажимали "Fetch" до этого
![gh.png](service/gh.png)

### Про ветки 
- По умолчанию используем ветку `main`, чтобы не усложнять себе жизнь.

## Горячие клавиши
- `Ctrl + O` — открыть навигатор файлов, чтобы создать новый файл
- `Ctrl + S` — линтер, автоматическое форматирование
- `Ctrl + Shift + 8` — создать сноску
- `Ctrl + Shift + E` — вставить цитирование
Остальные можно посмотреть в настройках, во вкладке Hotkeys (нажать на иконку фильтра и выбрать Assigned).
