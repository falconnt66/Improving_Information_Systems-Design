<H1>Сети внутри сетей</H1>
Примеры

<H2>Язык спецификации CO-OPN</H2> (параллельные объектно-ориентированные сети Петри) основан как на алгебраических спецификациях, так и на формализмах алгебраических сетей Петри. Первый формализм представляет аспекты структур данных, а второй - поведенческие и параллельные аспекты систем. Для работы с большими спецификациями были введены некоторые возможности структурирования. Была принята объектно-ориентированная парадигма, что означает, что спецификация CO-OPN - это совокупность объектов, которые взаимодействуют одновременно. Взаимодействие между объектами достигается посредством механизма синхронизации, то есть каждое событие объекта может запрашивать синхронизацию с некоторыми методами (параметризованными событиями) одного или группы партнеров посредством выражения синхронизации.

Спецификация CO-OPN состоит из набора двух разных модулей: модулей абстрактного типа данных и объектных модулей. Модули абстрактного типа данных относятся к компоненту структуры данных спецификаций, и при описании этих модулей используется множество отсортированных алгебраических спецификаций. Кроме того, объектные модули представляют собой концепцию инкапсулированных сущностей, которые обладают внутренним состоянием и предоставляют внешнему виду различные услуги. Для этого второго типа модулей был принят формализм алгебраической сети. Алгебраические сети Петри, своего рода сети высокого уровня, являются большим улучшением по сравнению с сетями Петри, то есть токены сетей Петри заменены структурами данных, которые описываются с помощью алгебраических абстрактных типов данных. Для управления видимостью как модули абстрактного типа данных, так и объектные модули состоят из интерфейса (который позволяет некоторым операциям быть видимыми снаружи) и тела (который в основном инкапсулирует свойства операций и некоторые операции, которые используются для построения модели) . В случае модулей объектов состояние и поведение объектов остаются скрытыми внутри секции тела.

Для разработки моделей с использованием языка CO-OPN можно использовать структуру COOPNBuilder [1], которая представляет собой среду, состоящую из набора инструментов, предназначенных для поддержки параллельной разработки программного обеспечения на основе языка CO-OPN.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<H2>Renew</H2> - это редактор и симулятор мультиформализма на основе Java, который обеспечивает гибкий подход к моделированию, основанный, но не ограничиваясь, ссылочными сетями.

Сети Петри - хорошо зарекомендовавшие себя средства для описания параллельных систем. За прошедшие годы были предложены многочисленные расширения базового формализма для учета абстрактных типов данных, объектной ориентации, иерархий или новых типов дуги.

Среди них - формализм ссылочных сетей, где токены могут быть ссылками на произвольные объекты, особенно на другие сети, что позволяет использовать вложенные сетевые модели. Он позволяет создавать надписи Java, имеет встроенные типы List и Tuple, предлагает тестовые, ингибирующие и гибкие дуги и имеет мощный механизм синхронизации.
