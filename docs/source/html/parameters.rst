:orphan:

.. title:: Globalizer: Параметры командной строки

Параметры командной строки
==========================

.. container:: doxygen-content

   Таблица 1. Параметры командной строки
   -------------------------------------

   .. list-table::
      :widths: 10 15 8 12 15 40
      :header-rows: 1

      * - Короткий параметр
        - Полное имя параметра
        - Тип
        - Значение по умолчанию
        - Диапазон / Примечания
        - Описание
      * - ``-HELP``
        - ``-HELP``
        - flag
        - ``0``
        - —
        - Распечатать справку
      * - ``-PLOT``
        - ``-IsPlot``
        - flag
        - ``0``
        - —
        - Нарисовать график функции
      * - ``-ShowFigure``
        - ``-ShowFigure``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Открыть рисунок в интерактивном окне
      * - ``-HideTrialsPoints``
        - ``-HideTrialsPoints``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Скрыть точки испытаний на графике
      * - ``-FigureType``
        - ``-FigureType``
        - enum
        - ``0`` (``LevelLayers``)
        - см. Таблицу 2
        - Тип визуализации целевой функции
      * - ``-CalcsType``
        - ``-CalcsType``
        - enum
        - ``0`` (``ObjectiveFunction``)
        - см. Таблицу 2
        - Тип вычислений для визуализации
      * - ``-PGS``
        - ``-PlotGridSize``
        - int
        - ``300``
        - ``>0``
        - Плотность сетки рисования
      * - ``-PlotFileName``
        - ``-PlotFileName``
        - string
        - ``""``
        - Любая строка без пробелов
        - Имя файла для сохранения изображения
      * - ``-ICNP``
        - ``-IsCalculateNumPoint``
        - flag
        - ``0``
        - —
        - Число испытаний за итерацию вычисляется на каждой итерации
      * - ``-np``
        - ``-NumPoints``
        - int
        - ``1``
        - ``>0``
        - Число точек, порождаемых методом на одной итерации
      * - ``-spm``
        - ``-StepPrintMessages``
        - int
        - ``100000``
        - ``>0``
        - Шаг печати информации в консоль
      * - ``-ssp``
        - ``-StepSavePoint``
        - int
        - ``1000000``
        - ``>0``
        - Через сколько итераций сохранять точки
      * - ``-tm``
        - ``-TypeMethod``
        - enum
        - ``0`` (``StandartMethod``)
        - см. Таблицу 2
        - Тип метода АГП
      * - ``-tc``
        - ``-TypeCalculation``
        - enum
        - ``0`` (``OMP``)
        - см. Таблицу 2
        - Организация проведения испытаний
      * - ``-tp``
        - ``-TypeProcess``
        - enum
        - ``0`` (``SynchronousProcess``)
        - см. Таблицу 2
        - Тип процесса
      * - ``-nt``
        - ``-NumThread``
        - int
        - ``1``
        - ``>0``
        - Число OpenMP потоков
      * - ``-sb``
        - ``-SizeInBlock``
        - int
        - ``32``
        - ``>0``
        - Размер CUDA блока
      * - ``-IsPF``
        - ``-IsPrintFile``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Печатать отчёт в файл
      * - ``-ResulLog``
        - ``-ResulLog``
        - string
        - ``"000"``
        - ``"000"`` — не печатать
        - Файл для печати результата
      * - ``-N``
        - ``-Dimension``
        - int
        - ``1``
        - ``>0``
        - Размерность задачи
      * - ``-r``
        - ``-r``
        - double
        - ``4.0``
        - ``>1``
        - Надёжность метода
      * - ``-rd``
        - ``-rDynamic``
        - double
        - ``0``
        - Любое
        - Добавка при динамическом изменении r
      * - ``-rE``
        - ``-rEps``
        - double
        - ``0.01``
        - ``>0``
        - Параметр eps-резервирования
      * - ``-Comment``
        - ``-Comment``
        - string
        - ``"000"``
        - Любая строка без пробелов
        - Комментарий к эксперименту
      * - ``-E``
        - ``-Epsilon``
        - double
        - ``0.01``
        - ``>0``
        - Единая точность
      * - ``-M_constant``
        - ``-M_constant``
        - double[]
        - ``1``
        - ``>0``
        - Начальные оценки констант Гёльдера
      * - ``-m``
        - ``-m``
        - int
        - ``10``
        - ``>1``
        - Плотность построения развёртки (точность ``1/2^m``)
      * - ``-dc``
        - ``-deviceCount``
        - int
        - ``-1``
        - ``>= -1``
        - Количество ускорителей (``-1`` — авто)
      * - ``-mt``
        - ``-MapType``
        - enum
        - ``0`` (``mpBase``)
        - см. Таблицу 2
        - Тип развёртки
      * - ``-tdsp``
        - ``-TypeDistributionStartingPoints``
        - enum
        - ``0`` (``Evenly``)
        - см. Таблицу 2
        - Тип распределения начальных точек
      * - ``-dac``
        - ``-DebugAsyncCalculation``
        - int
        - ``0``
        - ``0/1``
        - Отладка асинхронной схемы
      * - ``-IsPSP``
        - ``-IsPrintSectionPoint``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Печатать информацию о сечении
      * - ``-MaxNP``
        - ``-MaxNumOfPoints``
        - int
        - ``1000000``
        - ``>0``
        - Макс. число итераций для процессов
      * - ``-sd``
        - ``-IsSetDevice``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Назначать процессу своё устройство
      * - ``-di``
        - ``-deviceIndex``
        - int
        - ``-1``
        - ``>= -1``
        - Индекс устройства (``-1`` — авто)
      * - ``-doLV``
        - ``-localRefineSolution``
        - enum
        - ``0`` (``None``)
        - см. Таблицу 2
        - Способ использования локального метода
      * - ``-tlm``
        - ``-TypeLocalMethod``
        - enum
        - ``0`` (``HookeJeeves``)
        - см. Таблицу 2
        - Тип локального метода
      * - ``-lvi``
        - ``-localIteration``
        - int
        - ``10000``
        - ``>0``
        - Итераций локального метода
      * - ``-lve``
        - ``-localVerificationEpsilon``
        - double
        - ``0.0001``
        - ``>0``
        - Точность локального метода
      * - ``-lvnp``
        - ``-localVerificationNumPoint``
        - int
        - ``1``
        - ``>0``
        - Кол-во точек для локального метода
      * - ``-hdsic``
        - ``-HDSolverIterationCount``
        - int
        - ``1``
        - ``>0``
        - Итерации решателя больших задач
      * - ``-lm``
        - ``-localMix``
        - int
        - ``0``
        - ``>= 0``
        - Параметр смешивания
      * - ``-la``
        - ``-localAlpha``
        - double
        - ``15``
        - ``>0``
        - Степень локальной адаптации
      * - ``-sepS``
        - ``-sepS``
        - enum
        - ``0`` (``Off``)
        - см. Таблицу 2
        - Сепарабельный поиск на старте
      * - ``-rndS``
        - ``-rndS``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Случайный поиск на старте
      * - ``-lib``
        - ``-libPath``
        - string
        - ``DEFAULT_LIB``
        - Путь к ``.dll``/``.so``
        - Путь к библиотеке с задачей
      * - ``-libConf``
        - ``-libConfigPath``
        - string
        - ``""``
        - Путь к ``.xml``
        - Путь к конфигу задачи
      * - ``-stopCond``
        - ``-stopCondition``
        - enum
        - ``0`` (``Accuracy``)
        - см. Таблицу 2
        - Тип критерия остановки
      * - ``-isbal``
        - ``-isStopByAnyLevel``
        - bool
        - ``true``
        - ``0/1``, ``false/true``
        - Критерий применим к любому уровню
      * - ``-isPRC``
        - ``-isPrintResultToConsole``
        - bool
        - ``true``
        - ``0/1``, ``false/true``
        - Печать результатов в консоль
      * - ``-sip``
        - ``-iterPointsSavePath``
        - string
        - ``""``
        - Путь к файлу
        - Путь сохранения точек
      * - ``-advInf``
        - ``-printAdvancedInfo``
        - flag
        - ``0``
        - —
        - Печать доп. статистики
      * - ``-dpp``
        - ``-disablePrintParameters``
        - flag
        - ``0``
        - —
        - Отключить печать параметров
      * - ``-logFName``
        - ``-logFileNamePrefix``
        - string
        - ``"globalizer_log"``
        - Любая строка без пробелов
        - Префикс имени лог-файла
      * - ``-ca``
        - ``-calculationsArray``
        - int[]
        - ``-1``
        - ``-1, 0, 1, 2``
        - Распределение типов вычислений
      * - ``-ts``
        - ``-TypeSolver``
        - enum
        - ``0`` (``SingleSearch``)
        - см. Таблицу 2
        - Тип решателя
      * - ``-dt``
        - ``-DimInTask``
        - int[]
        - ``[0,0,0,0]``
        - ``>= 0``
        - Размерности подзадач
      * - ``-mbs``
        - ``-mpiBlockSize``
        - int
        - ``1``
        - ``>0``
        - Размер блока в MPI
      * - ``-iutr``
        - ``-isUseTaskR``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Использовать R как характеристику задачи
      * - ``-iufr``
        - ``-isUseFullRecount``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Глобальный пересчёт M или Z
      * - ``-iuir``
        - ``-isUseIntervalR``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - R как характеристика интервалов
      * - ``-iugz``
        - ``-isUseGlobalZ``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Использовать глобальное Z
      * - ``-inuz``
        - ``-isNotUseZ``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Не использовать Z
      * - ``-talp``
        - ``-TypeAddLocalPoint``
        - enum
        - ``1`` (``NotTakenIntoAccount...``)
        - см. Таблицу 2
        - Тип добавления точек лок. уточнения
      * - ``-mclp``
        - ``-maxCountLocalPoint``
        - int
        - ``5``
        - ``>0``
        - Макс. точек от лок. метода
      * - ``-icibp``
        - ``-isCalculationInBorderPoint``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Вычислять в крайних точках
      * - ``-ltt``
        - ``-LocalTuningType``
        - enum
        - ``0`` (``WithoutLocalTuning``)
        - см. Таблицу 2
        - Тип локального уточнения
      * - ``-ltXi``
        - ``-ltXi``
        - double
        - ``1e-6``
        - ``>0``
        - Параметр ξ для уточнения
      * - ``-islfp``
        - ``-isLoadFirstPointFromFile``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Загружать нач. точки из файла
      * - ``-fpf``
        - ``-FirstPointFilePath``
        - string
        - ``""``
        - Путь к файлу
        - Путь к файлу с нач. точками
      * - ``-ProcRank``
        - ``-ProcRank``
        - int
        - ``-1``
        - ``>= -1``
        - Ранг процесса (только чтение)
      * - ``-fsm``
        - ``-functionSignMultiplier``
        - double[]
        - ``[1.0,1.0,1.0,1.0]``
        - Любое
        - Множитель (мин/макс)
      * - ``-sp``
        - ``-startPoint``
        - double[]
        - ``MaxDouble``
        - Любое
        - Начальная точка
      * - ``-spv``
        - ``-startPointValues``
        - double[]
        - ``MaxDouble``
        - Любое
        - Значения в нач. точке
      * - ``-IsUSP``
        - ``-IsUseStartPoint``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Использовать стартовую точку из задачи
      * - ``-IsUEC``
        - ``-IsUseExtendedConsole``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Расширенный консольный интерфейс
      * - ``-IsAPS``
        - ``-automaticParametersSetting``
        - bool
        - ``false``
        - ``0/1``, ``false/true``
        - Автонастройка параметров
      * - ``-fs``
        - ``-fileSerializer``
        - string
        - ``""``
        - Путь к файлу
        - Путь для сохранения/загрузки
      * - ``-MIWI``
        - ``-MaxIterationsWithoutImprovement``
        - int
        - ``100``
        - ``>0``
        - Макс. итераций без улучшения
      * - ``-IC``
        - ``-iterationsCount``
        - int
        - ``1000000``
        - ``>0``
        - Макс. итераций (авторежим)

   Таблица 2. Возможные значения параметров типа ``enum``
   -------------------------------------------------------

   .. list-table::
      :widths: 20 40 40
      :header-rows: 1

      * - Полное имя параметра
        - Возможные значения (``enum``)
        - Расшифровка / Описание
      * - ``-FigureType``
        - ``0`` = ``LevelLayers``\n``1`` = ``Surface``
        - ``0`` — линии уровней\n``1`` — поверхность
      * - ``-CalcsType``
        - ``0`` = ``ObjectiveFunction``\n``1`` = ``Approximation``\n``2`` = ``Interpolation``\n``3`` = ``ByPoints``\n``4`` = ``OnlyPoints``
        - ``0`` — построение по сетке 100×100\n``1`` — аппроксимация по поисковой информации\n``2`` — интерполяция по поисковой информации\n``3`` — «натягивание» на точки без сглаживания\n``4`` — только распределение точек
      * - ``-TypeMethod``
        - ``0`` = ``StandartMethod``\n``1`` = ``IntegerMethod``\n``2`` = ``RSAMethod``
        - ``0`` — базовый АГП\n``1`` — метод для смешанных задач\n``2`` — метод RSA
      * - ``-TypeCalculation``
        - ``0`` = ``OMP``\n``1`` = ``CUDA``\n``2`` = ``MPI_calc``\n``3`` = ``AsyncMPI``\n``4`` = ``OneApi``
        - ``0`` — OpenMP (CPU)\n``1`` — CUDA (GPU NVIDIA)\n``2`` — синхронный MPI\n``3`` — асинхронный MPI\n``4`` — Intel oneAPI
      * - ``-TypeProcess``
        - ``0`` = ``SynchronousProcess``
        - ``0`` — синхронный процесс (единственный в текущей версии)
      * - ``-MapType``
        - ``2`` = ``mpBase``
        - ``2`` — базовая одиночная развёртка (единственная в текущей версии)
      * - ``-TypeDistributionStartingPoints``
        - ``0`` = ``Evenly``
        - ``0`` — равномерное распределение (единственное)
      * - ``-localRefineSolution``
        - ``0`` = ``None``\n``1`` = ``FinalStart``\n``2`` = ``UpdatedMinimum``
        - ``0`` — без локального метода\n``1`` — запуск по завершению АГП\n``2`` — запуск при обновлении лучшей точки
      * - ``-TypeLocalMethod``
        - ``0`` = ``HookeJeeves``\n``1`` = ``LeastSquareMethod``\n``3`` = ``ParallelHookeJeeves``
        - ``0`` — метод Хука-Дживса\n``1`` — метод наименьших квадратов\n``3`` — параллельный метод Хука-Дживса
      * - ``-sepS``
        - ``0`` = ``Off``\n``1`` = ``GridSearch``\n``2`` = ``GlobalMethod``
        - ``0`` — выключен\n``1`` — поиск по равномерной сетке\n``2`` — АГП по каждой переменной
      * - ``-stopCondition``
        - ``0`` = ``Accuracy``\n``1`` = ``OptimumVicinity``\n``2`` = ``OptimumVicinity2``\n``3`` = ``OptimumValue``\n``4`` = ``MaxIterWithoutImprovement``\n``5`` = ``InLocalArea``
        - ``0`` — по длине интервала < eps\n``1`` — попадание в окрестность eps * размер области\n``2`` — попадание в окрестность eps\n``3`` — совпадение значения критерия с eps\n``4`` — макс. итераций без улучшения\n``5`` — попадание в локальную область
      * - ``-TypeSolver``
        - ``0`` = ``SingleSearch``\n``2`` = ``HDSearch``
        - ``0`` — классический АГП\n``2`` — решатель задач большой размерности
      * - ``-TypeAddLocalPoint``
        - ``0`` = ``RegularPoints``\n``1`` = ``NotTakenIntoAccountInStoppingCriterion``\n``2`` = ``IntegratedOnePoint``\n``3`` = ``IntegratedAllPoint``\n``4`` = ``IntegratedBestPath``
        - ``0`` — как обычные точки\n``1`` — не учитывать в критерии остановки\n``2`` — добавить одну точку\n``3`` — добавить все точки\n``4`` — добавить точки из лучшей траектории
      * - ``-LocalTuningType``
        - ``0`` = ``WithoutLocalTuning``\n``1`` = ``MiniMax``\n``2`` = ``Adaptive``\n``3`` = ``AdaptiveMiniMax``
        - ``0`` — без уточнения\n``1`` — минимаксное\n``2`` — адаптивное\n``3`` — адаптивно-минимаксное