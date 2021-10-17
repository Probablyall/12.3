### Известно:
* база данных должна быть отказоустойчивой (не менее трех копий, master-slave) и потребляет около 4 ГБ ОЗУ в работе;
* кэш должен быть аналогично отказоустойчивый, более трех копий, потребление: 4 ГБ ОЗУ, 1 ядро;
* фронтенд обрабатывает внешние запросы быстро, отдавая статику: не более 50 МБ ОЗУ на каждый экземпляр;
* бекенду требуется больше: порядка 600 МБ ОЗУ и по 1 ядру на копию.

Требования: опишите, сколько нод в кластере и сколько ресурсов (ядра, ОЗУ, диск) нужно для запуска приложения. Расчет вести из необходимости запуска 5 копий фронтенда и 10 копий бекенда, база и кеш.

Где данных из условия не хватало, вписывал то, что больше подходит по моему мнению.

### Ресурсы для приложений:
![tabl1.PNG](https://github.com/Probablyall/12.3/blob/main/tabl1.PNG)

### Иные необходимые ресурсы:
![tabl2.PNG](https://github.com/Probablyall/12.3/blob/main/tabl2.PNG)

Worker node - здесь приложения, которые необходимы для работы кластера Calico, Prometheus, Centralized logging.

OS - ОС на которой развернут кластер.

### Итого
#### HDD: 212 Гб
#### ОЗУ: 120 Гб
#### ЦПУ: 101
