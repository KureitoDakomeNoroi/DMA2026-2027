# Практическая работа №8: Объектно-ориентированное программирование в Dart

## Тема 1. Классы, инкапсуляция, методы и геттеры/сеттеры

### Задание 1

Создайте класс `Thermostat` с приватным полем `_temperatureCelsius`. Реализуйте геттер температуры в градусах Фаренгейта и сеттер с ограничением диапазона от -50 до +100 °C.

![alt text](image.png)

### Задание 2

Разработайте класс `Pedometer`, где текущие шаги можно только увеличивать через метод `addSteps(int count)`, а уменьшать нельзя.

![alt text](image-1.png)

### Задание 3

Класс `Book` содержит поля названия и числа страниц. Добавьте вычисляемый геттер `estimatedReadingHours`, считающий время из расчета 1 страница в 2 минуты.

![alt text](image-2.png)

### Задание 4

Класс `UserCredentials` с приватным паролем `_passwordHash`. Сеттер принимает сырую строку, проверяет ее длину (\(\ge 8\) символов) и сохраняет псевдо-хэш.

![alt text](image-3.png)

### Задание 5

Добавьте в класс `DeviceSession` статическое поле `static int activeSessionsCount`, которое увеличивается при создании каждого нового объекта.

![alt text](image-4.png)

## Тема 2. 

### Задание 1

Создайте класс `AppColor` с конструкторами `AppColor.fromHex(String hex)` и `AppColor.fromRGBO(int r, int g, int b, double o)`.

![alt text](image-5.png)

### Задание 2

Создайте класс `const Point2D(this.x, this.y)`. Создайте два идентичных константных объекта и убедитесь, что `identical(p1, p2) == true`.

![alt text](image-6.png)

### Задание 3

**Список инициализации с assert:** Создайте класс `Rectangle` с полями ширины и высоты. В списке инициализации добавьте проверку `assert(width > 0 && height > 0)`.

![alt text](image-7.png)

### Задание 4

Реализуйте класс `ApiClient` с фабричным конструктором `factory ApiClient()`, гарантированно возвращающим один и тот же приватный экземпляр.

![alt text](image-8.png)

### Задание 5

 Напишите класс `Circle(this.radius)` и именованный конструктор `Circle.unit() : this(1.0);`, перенаправляющий вызов на основной.

![alt text](image-9.png)

## Тема 3. 

### Задание 1

 Создайте базовый класс `Card` и наследников `DebitCard` (без овердрафта) и `CreditCard` (с лимитом овердрафта).

![alt text](image-10.png)

### Задание 2

Создайте список `List<BaseScreen>` и в цикле вызовите метод `render()` для каждого элемента независимо от конкретного подтипа.

![alt text](image-11.png)

### Задание 3

Перепишите конструктор наследника с использованием компактного синтаксиса `SubClass({required super.id, super.title});`.

![alt text](image-12.png)

### Задание 4

Покажите пример сужения типа аргумента в переопределенном методе подкласса с помощью ключевого слова `covariant`.

![alt text](image-13.png)

### Задание 5

Создайте метод критической проверки лицензии в базовом классе и запретите его изменение в наследниках.

![alt text](image-14.png)

## Тема 4. 

### Задание 1

Объявите интерфейс `StorageService` с методами `save(String key, String val)`, `read(String key)`, `delete(String key)`. Реализуйте класс `MemoryStorageService` через `implements`.

![alt text](image-15.png)

### Задание 2

Создайте класс `SmartTv`, реализующий сразу два несвязанных интерфейса: `Displayable` и `NetworkConnectable`.

![alt text](image-16.png)

### Задание 3

Создайте `sealed class AuthState` с наследниками `Unauthenticated`, `Authenticating`, `Authenticated(User user)` и `AuthFailed(String reason)`.

![alt text](image-17.png)

### Задание 4

Создайте класс `base class Engine`, гарантирующий, что сторонние библиотеки смогут только наследовать его (`extends`), но не смогут реализовать его как чистый интерфейс (`implements`).

![alt text](image-18.png)

### Задание 5

Создайте чистый интерфейсный контракт, исключающий прямое наследование реализации вне родной библиотеки.

![alt text](image-19.png)

## Тема 5. 

### Задание 1

Создайте миксин `JsonPrintable`, добавляющий любому классу метод `printAsJson()`.

![alt text](image-20.png)

### Задание 2

Создайте миксин `AutoDisposer on ChangeNotifier`, добавляющий флаг `bool isDisposed` и проверяющий его в методах.

![alt text](image-21.png)

### Задание 3

Напишите миксин `AnalyticsTracker` с методом `trackEvent(String eventName)` и примените его к классу кнопки `CustomButton`.

![alt text](image-22.png)

### Задание 4

Создайте класс с двумя миксинами, реализующими одинаковый метод `execute()`. Покажите на практике, метод какого миксина выполнится первым (принцип правого приоритета).

![alt text](image-23.png)

### Задание 5

Создайте миксин `MemoizationMixin`, сохраняющий результаты тяжелых математических функций в словарь по строковому ключу аргументов.

![alt text](image-24.png)


### Блок 1: 

#### Задание 1

Создайте константную модель товара с обязательными полями, расчетом цены со скидкой и валидацией неотрицательной стоимости в списке инициализации.

![alt text](image-25.png)

#### Задание 2

Реализуйте конструктор `User.fromJson(Map<String, dynamic> json)` с обработкой отсутствующих полей и защитой от `TypeError`.

![alt text](image-26.png)

#### Задание 3

Спроектируйте класс `AppLocale` с фабричным конструктором, возвращающим единственный экземпляр для каждого языка: `AppLocale("ru")`, `AppLocale("en")`.

![alt text](image-27.png)

#### Задание 4

Класс `GeoPoint` с именованным конструктором `GeoPoint.fromString("55.751244, 37.618423")`.

![alt text](image-28.png)

#### Задание 5

Напишите фабричный конструктор `ContactCard.fromDatabaseRecord(Map<String, Object?> row)`.

![alt text](image-29.png)

#### Задание 6

Добавьте метод `UserModel copyWith({String? name, String? avatarUrl})` для неизменяемой модели.

![alt text](image-30.png)

#### Задание 7

Класс `DateRange(this.start, this.end)` со списком инициализации, выбрасывающим `AssertionError`, если дата окончания раньше даты начала.

![alt text](image-31.png)

#### Задание 8

Класс `TransactionDto` с именованными конструкторами для пополнения (`TransactionDto.deposit`), списания (`TransactionDto.withdrawal`) и перевода (`TransactionDto.transfer`).

![alt text](image-32.png)

#### Задание 9

Фабричный конструктор `EnvConfig.fromEnvironment()`, читающий флаги через `const String.fromEnvironment()`.

![alt text](image-33.png)

#### Задание 10

Переопределите оператор `==` и метод `hashCode` для класса `CartItem` на основе совпадения полей `productId` и `selectedSize`.

![alt text](image-34.png)

### Блок 2:

#### Задание 1

 Базовый класс `InAppNotification` (таймаут, заголовок) и наследники `SuccessNotification`, `WarningNotification`, `CriticalAlertNotification` с разным цветом и иконкой.

![alt text](image-36.png)

#### Задание 2

 Базовый класс `BaseDialog` с шаблоном отрисовки шапки и подвала, и наследник `ConfirmActionDialog` с кнопками «Подтвердить» и «Отмена».

![alt text](image-37.png)

#### Задание 3

 Базовый класс `MediaPlayer` (методы `play()`, `pause()`, `seek()`) и специализированные наследники `AudioPlayer` и `HlsVideoPlayer`.

![alt text](image-38.png)

#### Задание 4

 Базовый класс `HardwareSensor` и подклассы `AccelerometerSensor` (оси X, Y, Z) и `BarometerSensor` (давление в гПа).

![alt text](image-39.png)

#### Задание 5

 Базовый класс `SubscriptionPlan` и наследники `MonthlyPlan`, `AnnualDiscountPlan` (скидка 20%) и `FamilyPlan` (множитель цены за участников).

![alt text](image-40.png)

#### Задание 6

 Базовый класс `CanvasLayer` (прозрачность, видимость, z-index) и подклассы `VectorLayer`, `RasterBitmapLayer`, `TextLayer`.

![alt text](image-41.png)

#### Задание 7

Базовый класс `PaymentGateway` с защищенным методом логирования и наследники `SbpGateway` (Система быстрых платежей) и `BankCardGateway`.

![alt text](image-42.png)

#### Задание 8

Базовый экран обучающего тура с кнопкой пропуска и конкретные шаги с уникальными иллюстрациями.

![alt text](image-43.png)

#### Задание 9

Базовый класс `WidgetButton` и подкласс `AsyncLoadingButton`, отображающий индикатор загрузки при активном асинхронном действии.

![alt text](image-44.png)

#### Задание 10

Базовый класс `AppLogger` и подклассы `ConsoleLogger` (форматированный вывод в терминал) и `FileCrashLogger` (запись на диск).

![alt text](image-45.png)

### Блок 3:

#### Задание 1

Объявите интерфейс `ProductRepository` с методами `Future<List<Product>> getAll()`, `Future<Product> getById(int id)` и создайте две реализации: `NetworkProductRepository` и `MockProductRepository`.

![alt text](image-46.png)

#### Задание 2

Спроектируйте интерфейс `BiometricAuthService` с методами `canAuthenticate()` и `authenticate()`. Напишите реализацию-заглушку для тестов.

![alt text](image-47.png)

#### Задание 3

Интерфейс `CryptoService` с методами `encrypt(String plainText)` и `decrypt(String cipherText)`. Реализуйте класс `AesCryptoService`.

![alt text](image-48.png)

#### Задание 4

 Интерфейс `AnalyticsProvider` с методом `logEvent(String name, Map<String, Object> params)`. Реализуйте множественную отправку через класс `CompositeAnalyticsProvider`.

![alt text](image-49.png)

#### Задание 5

 Спроектируйте контракт получения координат устройства с поддержкой стрима обновлений позиции `Stream<GeoPoint> get positionStream`.

![alt text](image-50.png)

#### Задание 6

Интерфейс `NotificationSender` с методами отправки мгновенных и отложенных системных пушей.

![alt text](image-51.png)

#### Задание 7

Абстрактный класс `DataSyncEngine` с абстрактными методами `fetchRemoteDelta()` и `applyLocalChanges()`.

![alt text](image-52.png)

#### Задание 8

Интерфейс `ConnectivityService` с геттером `bool isOnline` и стримом событий потери интернета.

![alt text](image-53.png)

#### Задание 9

Спроектируйте интерфейс с обобщенными методами `T? read<T>(String key)` и `Future<void> write<T>(String key, T value)`.

![alt text](image-54.png)

#### Задание 10

Контракт `ReportExporter` с реализациями `PdfReportExporter` и `ExcelReportExporter`.

![alt text](image-55.png)

### Блок 4: 

#### Задание 1

Миксин `DebounceMixin`, предотвращающий повторный вызов одного и того же действия чаще чем раз в 500 мс.

![alt text](image-56.png)

#### Задание 2

Миксин, автоматически сохраняющий текстовые поля ввода при сворачивании приложения.

![alt text](image-57.png)

#### Задание 3

 Миксин `NetworkAwareMixin`, внедряющий в презентер экрана проверку доступности интернета перед выполнением любого запроса.

![alt text](image-58.png)

#### Задание 4

 Миксин `CurrencyFormatterMixin`, предоставляющий готовый метод преобразования чисел в красивый денежный формат.

![alt text](image-59.png)

#### Задание 5

Миксин `PeriodicRefreshMixin`, запускающий периодический опрос сервера каждые 30 секунд при активном экране.

![alt text](image-60.png)

#### Задание 6

 Миксин `PassportValidationMixin` с методами строгой проверки серии, номера и кода подразделения.

![alt text](image-61.png)

#### Задание 7

Подмешиваемый контроллер управления прозрачностью элемента от 0.0 до 1.0.

![alt text](image-62.png)

#### Задание 8

Миксин, предоставляющий экрану быстрый доступ к текущей цветовой палитре (темная/светлая).

![alt text](image-63.png)

#### Задание 9

Миксин, парсящий входящие URI-схемы приложения и открывающий целевые экраны.

![alt text](image-64.png)

#### Задание 10

 Подмешиваемый модуль, отправляющий критические действия модератора на выделенный сервер безопасности.

![alt text](image-65.png)

### Блок 5: 

#### Задание 1

Создайте `sealed class CartState` с состояниями: `CartEmpty`, `CartLoading`, `CartLoaded(List<Item> items, double total)`, `CartCheckoutError(String error)`. Напишите функцию обработки состояний через исчерпывающий `switch`.

![alt text](image-66.png)

#### Задание 2

 Реализуйте `sealed class Result<T>` с подтипами `Success<T>(final T data)` и `Failure<T>(final Exception exception)`.

![alt text](image-67.png)

#### Задание 3

 Создайте `sealed class LoginEvent` с событиями `LoginEmailChanged(String email)`, `LoginPasswordChanged(String pass)`, `LoginSubmitted`.

![alt text](image-68.png)

#### Задание 4

 Объявите класс `final class EncryptionKey`, запретив любое его расширение или реализацию вне текущей библиотеки.

![alt text](image-69.png)

#### Задание 5

 Разработайте интерфейсный класс платежного терминала, запретив прямое наследование логики клиентами библиотеки.

![alt text](image-70.png)

#### Задание 6

 Спроектируйте `sealed class AppRoute` для типобезопасной навигации во Flutter.

![alt text](image-71.png)

#### Задание 7

 Создайте абстрактный класс `Command` с методом `execute()` и `undo()` для реализации функции отмены действий в редакторе текста.

![alt text](image-72.png)
![alt text](image-73.png)

#### Задание 8

Реализуйте `NotificationBuilder` с цепочечными вызовами `.setTitle().setBody().setIcon().build()`.

![alt text](image-74.png)

#### Задание 9

 Создайте легковесную шину событий с классами событий и методами подписки/отписки.

![alt text](image-75.png)

#### Задание 10

- Спроектируйте `sealed class TaxiOrderState` (поиск машины, машина назначена, поездка, завершено, отменено).
- Создайте класс заказа `TaxiOrder` с именованными фабричными конструкторами и списком инициализации.
- Реализуйте миксины `LocationTrackingMixin` и `FareCalculationMixin`.
- Напишите контроллер управления поездкой с исчерпывающим сопоставлением с шаблонами.

![alt text](image-76.png)
![alt text](image-77.png)
![alt text](image-78.png)
