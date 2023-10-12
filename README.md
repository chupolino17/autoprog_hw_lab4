
# Лабораторная работа 4


1. Реализованная спецификация для 4ех организаций [спецификаия.](./prog-autom-consensus-analyzer/resources/cnf-4-orgs.yaml)
2. [График](./prog-autom-consensus-analyzer/results/cnf-4-true/graph.png) зависимости вероятности подтверждения от среднего числа
сообщений. 
3. Код getRequest реализован в файлк [SendingConfirmationServiceImplTest.java](./consensus-scheduler/src/test/java/SendingConfirmationServiceImplTest.java) шедулера.
4. Вывод планировщика лежит в [папке](./consensus-scheduler/target/test-classes).

### Ответы на вопросы:
1. В моем понимании главная цель, проследить зависимость вероятности подтверждения от кол-ва сообщений, при большой вероятности график разъедется.
2. Планировщик можно запускать несколько раз для одних и тех же результатов анализатора. Было бы странно каждый раз запускать анализатор, когда результаты явно не меняются.
3. На графике явно видно вокруг каких значений флуктурируют показания, флуктуации происходят из-за не единичной вероятности событий. А по высотам он расходится в зависимости от Org2, которая стоит особняком в спецификации. 
4. Применение моделей с обратными переходами увеличивает вероятность подтверждения транзакции в сети.
