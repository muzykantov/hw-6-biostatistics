## Домашнее задание 6
### Тема: расчет выборки при планировании исследования.

#### Цель
Научиться рассчитывать выборку для исследований с различными конечными точками.

#### Описание ДЗ
При выполнении этого домашнего задания вам необходимо посчитать выборки для различных типов точек. Напишите соответствующий код, пользуясь указанными формулами.

Пусть наш спонсор заинтересован, чтобы исследование имело 80% мощность, а уровень значимости — 5%, ожидаемый drop-out rate = 10%.

**Что нужно сделать:**
- (3 балла) Рассчитайте выборку для исследования терапевтической эквивалентности для двухпериодного cross-over дизайна. Из предыдущих исследований известно, что дисперсия составляет 20% \( \sigma_m = 0.20 \), а разница средних составляет −10% \( \varepsilon = \mu_{\text{test}} - \mu_{\text{reference}} \). Клиницисты сообщают нам, что клинически значимая разница составляет 25% \( \delta = 0.25 \).

Используйте следующую формулу:
$$
n_1 = n_2 = \frac{(Z_{\alpha / 2} + Z_\beta)^2 \sigma_m^2}{2 * (\delta - |\varepsilon|)^2}, \quad n = n_1 + n_2
$$

- (3 балла) Рассчитайте выборку для гипотезы non-inferiority для двухвыборочного параллельного дизайна. Пусть клинически значимая разница \( \delta = -0.1 \), то есть мы ожидаем разницу не меньше 10%, а долю ответов для тестового препарата \( p_2 = 0.65 \), в то время как нам известно из предыдущих исследований, что доля ответов у препарата сравнения составляет \( p_1 = 0.85 \). Соотношение групп равно \( k = 1 \).

Используйте следующую формулу:
$$
n_1 = n_2 = \frac{(Z_{\alpha / 2} + Z_\beta)^2 (p_1^*(1 - p_1) + p_2^*(1 - p_2))}{(p_1 - p_2 - \delta)^2}, \quad n = n_1 + n_2
$$

- (4 балла) Рассчитайте выборку для гипотезы equality для следующего исследования. Мы хотим сравнить новую терапию инфекции, присоединяющейся в больничных условиях у пациентов с ожогами, с золотым стандартом, основываясь на данных, анализируемых с помощью регрессии Кокса. Пусть отношение рисков «золотой стандарт / новая терапия», hazard ratio, HR = 2. Мы предполагаем, что 80% пациентов \( d = 0.8 \) могут столкнуться с этим заболеванием. Соотношения групп терапии равны \( p_1 = p_2 = 0.5 \).

Используйте следующую формулу:
$$
n_1 = n_2 = \frac{(Z_{\alpha

 / 2} + Z_\beta)^2}{\ln (HR)^2 p_1 p_2 d}, \quad n = n_1 + n_2
$$
