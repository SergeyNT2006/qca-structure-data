# QCA Structure & Data

**Project «Structure and Data»** — numerical framework for separating *emergent structure* from *contingent parameters* in particle physics.

> **Status:** v14.4 (final). Code accompanying the article *«Structure and Data: QCA as a framework for separating emergent structure and contingent parameters»*.

## Key idea

The universe might be a computation — we see only its output, not its hardware. In this framework we ask: *which properties of particle physics can be derived from local unitary rules (QCA), and which must be given as input parameters?*

## What this framework is NOT

Three points to prevent misunderstanding.

1. **Not a simulation.** There is no "simulator outside" that executes our world as a program. QCA is an **ontology**, not the simulation hypothesis: the claim is that physics *is* a local unitary rule, not that someone *computes* it. There is no "before the rule" and no "outside the rule" — only the rule.

2. **Not a theory of everything.** The framework classifies what is derivable from local unitarity and what must be given as input. It does not derive the Standard Model, gravity, or cosmology. Eight class A sectors, four class B checks, five class C negative controls, and **four** data classifications — this is the **full scope** of the work, no more.

3. **Not a claim that the substrate is directly knowable.** We see the "output" (physics) and classify it into structure and data. We do not see the "hardware". Whether the hardware exists, what it is, and how our output relates to it — the framework **leaves in brackets**, does not resolve. The structure/data classification works *inside* the output, regardless of what is behind it.

## Main results

| Sector | Emergent? | Precision | Notebook |
|---|---|---|---|
| 1D Dirac | ✅ | 10⁻¹⁵ | 01 |
| U(1) gauge (photon) | ✅ | 10⁻¹⁷ | 02 |
| SU(2) gauge (W/Z) | ✅ | 10⁻¹⁶ | 03 |
| Mass vs structure | ✅ | 10⁻¹⁶ | 04 |
| Higgs (BCS condensate) | ✅ | 0.1% | 05 |
| 2D Dirac (honeycomb) | ✅ | α = 1.01, isotropy 1.0000 | 06 |
| 2D square (contrast) | ❌ | ratio > 1.15 | 07 |
| 3D Dirac on 4D wall | ✅ | E₀ = 0, wall 51%, isotropy 1.0 | 08 |
| Quark mass SVD | data | rank-1 (99.7%), factor 2 | 09 |
| Base scan (leptons) | exploratory (not established) | base 15: dev = 0.028148; p_abs = 10/84 = 0.1190 | 10 |
| 4D wall geometry | ❌ (null) | no 1/32 in v_F or c | 11 |
| Particle–antiparticle | ✅ (structure) | m = m̄, CPT | 12 |
| Neutrino base scan | data (partial) | Σmν = 0.0608 eV (consistent with DESI) | 13 |
| Fundamental constants | ❌ (data) | no hidden grid | 14 |
| Speed of light | ✅ (structure) | c = 1 (emergent from locality) | 15 |
| Quantum entanglement | ✅ (structure) | CHSH = 2√2, C = 1 (preserved) | 16 |
| Pauli exclusion | ✅ (structure) | Exchange = -1 (fermions), +1 (bosons) | 17 |
| 3 Generations | ✅ (structure) | N walls → N modes (exact); 2D overlap | 18 |
| CP violation | ❌ (data) | J(δ) sine wave; phase is input | 19 |

**Bottom line:**

- **Structure** (gauge, Dirac, Higgs, CPT, speed of light, entanglement, Pauli, 3 generations) — emergent from QCA at machine precision.
- **Parameters** (masses, Yukawa, constants, CP phase) — data: incompressible, not rational, no natural unit.
- **Exploratory observation (not established):** base-15 preference for leptons. dev = 0.028148, p_abs = 10/84 = 0.1190 (best-of-39). Status: **not established** (deficit to suggestive threshold 5/84 = 0.0595). Quarks: MC mean at base 40 = 0.178335; deterministic dev_best39 = 0.174249; no base below 5%. Look-elsewhere ratio = 4.76 (the triplet {μ,b,t} at base 40 beats leptons 4.76×). Framework does **not** depend on base-15.

## Classification (19 notebooks)

Framework relies on:

- **8 independent structure derivations** (class A): nb01–06, nb08, nb18 Parts B–C;
- **4 consistency checks with QM** (class B): nb12, nb15–17;
- **5 negative controls** (class C): nb07, nb11, nb14, nb18 Part A, nb19 T0–T2;
- **4 data classifications** (data): nb09 (quark SVD), nb10 (base scan), nb13 (neutrinos), nb19 T4–T5 (CP phase).

*Counters do not overlap; negative controls are not counted as confirmation levels. nb18 is split: Part A — class C, Parts B–C — class A. nb19 is split: T0–T2 — class C, T4–T5 — data.*

## Current Status

### Notebook 10 — Base scan: EXPLORATORY (not established)

Statistic: pairwise log-ratios `m_j/m_i` (scale-invariant by construction). Base 15: dev = **0.028148 ± 1.6059×10⁻⁵** for leptons. Best-of-39 permutation test: p_abs = **10/84 = 0.1190**, rank of leptons = 10/84. Status: **not established** (suggestive floor 5/84 = 0.0595).

Quarks: MC mean at base 40 = **0.178335 ± 1.4605×10⁻²**; deterministic dev_best39 = **0.174249**; 0 bases below 5%. Look-elsewhere: triplet {μ,b,t} at base 40 gives dev = 0.005912, ratio 4.76× better than leptons.

Fixed base 15 (secondary, post-selection caveat): p_fixed = 1/84 = 0.0119. **Invalidated by post-selection** (base 15 was found by scanning these data). Not used in abstract or bottom line.

2.8% and Koide (K = 2/3) are not independent: integer exponents give K = 0.65591603, fractional parts give K = 0.66666378. Same evidence, two formulations.

**Source:** `nb10_pvalue_results.txt` (single source for all numbers above). **Figure:** `figures/10_base_scan.png`.

### Notebook 18 — Three Generations: ✅ CLOSED (Structure)

N walls → N modes exact in 1D SSH; 2D realized via overlap fermions (Ginsparg–Wilson residual ~3×10⁻¹⁵). Mechanism = structure. Number N = 3 is input.

**Figures:** `figures/18_partA_doubling.png`, `figures/18_partA_chiral.png`, `figures/18_partB_ssh.png`.

### Notebook 19 — CP Violation: ✅ CLOSED (Data)

T0–T2: CP conserved (1D, 2 generations) — class C negative control. T4: J(δ) ≠ 0 (3 generations, toy CKM). T5: Majorana invariant ≠ 0 (only relevant for 0νββ, not oscillations). Phase δ is input. **CP violation = data (4th data classification).**

**Figure:** `figures/19_cp_violation.png`.

## Limitations

1. QCA is a framework, not a "theory of everything".
2. All successful results reproduce known physics. No new predictions are made; Σmν = 0.0608 eV (nb13) is a **consistency check** with the DESI DR2 upper bound, not a prediction.
3. Yukawa couplings remain unexplained.
4. "4D operator" interpretation is philosophical.
5. **Base 15 for leptons is exploratory: p_abs = 10/84 = 0.1190, not established.** Look-elsewhere ratio 4.76. It does not support the framework's core thesis.
6. Neutrinos and constants do not follow the base-15 grid.
7. 3 generations: mechanism exact in 1D; 2D requires overlap fermions. Number N = 3 is input.
8. CP violation: framework can host it, but phase δ is input.
9. 2.8% base-15 deviation and Koide K = 2/3 are not independent (fractional exponents follow from K = 2/3 constraint).
10. **Look-elsewhere factor 4.76 is a lower bound on the family-wise correction.** It accounts only for the 39 bases in nb10, not for hypotheses tested in v1–v13 (Koide, SVD, DESI, alternative normalizations). The true family-wise correction is strictly larger than 4.76, so **p_abs = 0.1190 is a lower bound, not a full correction**. This makes the base-15 observation even less established, not more.
11. Robustness checks (seed, N_MC, mean-vs-max aggregation) are not performed in v14.4; roadmap in `nb10_pvalue.md` §6. To be included in v15.
12. **Multi-source cosmology is not tested.** The framework is agnostic about initial conditions: it does not distinguish single-source and multi-source initialization. Preliminary numerical tests (outside this article) show no significant signal; the result remains exploratory and is not part of the article.
13. **Bounce cosmology and pre-inflationary phases are not tested.** The framework does not predict initial conditions; they are classified as "data". Ekpyrotic/bounce models are compatible with the framework but not tested in it.
14. **Gravity is not tested.** Emergence of 1/r² from the QCA lattice is a task for a separate notebook (nb20, planned), not v14.4. The framework does not claim to derive GR, the equivalence principle, or quantum gravity.
15. **SM chiral left-handed doublets are not implemented.** Overlap fermions (nb18 Part C) provide the technology for exact chiral symmetry, but the specific embedding of SU(2)_L doublets in QCA is not done. This is a direction for v15+.

## Falsification criteria

The "structure vs data" thesis would be falsified if:

1. A statistically significant base is found for quarks (same method; p < 0.01);
2. Adding local unitary interactions (a) changes a sector's classification from structure to data, or (b) requires fitting a parameter previously reproduced without fitting;
3. CP phase is derived from QCA rules without free parameters.

None of the three has occurred. Base-15 for leptons does **not** pass criterion (i) at p < 0.01 — its p_abs = 0.1190 is far from it. This is consistent with the framework: base-15 was an exploratory observation, not a structural derivation.

## Repository structure

```text
qca-structure-data/
│
├── README.md                          # This file (v14.4, EN + RU)
├── CHANGELOG.md                       # R3–R18 traceability
├── nb10_pvalue.md                     # Pre-registration (fixed before run)
├── nb10_pvalue_results.txt            # Actual run output (single source)
├── LICENSE                            # MIT
├── requirements.txt
│
├── notebooks/
│   ├── 01..17_*.ipynb
│   ├── 18_three_generations.ipynb
│   └── 19_cp_violation.ipynb
│
├── data/
│   ├── quark_masses.csv
│   └── lepton_masses.csv
│
└── figures/
    ├── 01..17_*.png
    ├── 10_base_scan.png
    ├── 18_partA_doubling.png
    ├── 18_partA_chiral.png
    ├── 18_partB_ssh.png
    └── 19_cp_violation.png
```

## Requirements

- Python 3.10+
- numpy 1.26.4, scipy 1.11.4, matplotlib 3.8.4

## Status

- ✅ Notebooks 01–19 tested; results reproduce to stated precision
- ✅ Base-15: final permutation test completed (p_abs = 10/84, NOT established)
- ⏳ Zenodo DOI: ready to assign after v14.4 commit

## License

- **Code**: MIT
- **Text and figures**: CC BY 4.0

---

# QCA: Структура и Данные

**Проект «Структура и Данные»** — численный подход для разделения *эмерджентной структуры* и *контингентных параметров* в физике частиц.

> **Статус:** v14.4 (финал). Код к статье *«Структура и Данные: QCA как подход к разделению эмерджентной структуры и контингентных параметров»*.

## Основная идея

Вселенная может быть вычислением — мы видим только его выход, но не «железо». В этом подходе мы задаём вопрос: *какие свойства физики частиц выводимы из локальных унитарных правил (QCA), а какие должны быть заданы как входные параметры?*

## Что подход **не** утверждает

Три пункта, чтобы предотвратить недопонимание.

1. **Не симуляция.** Нет «симулятора снаружи», который исполняет наш мир как программу. QCA — это **онтология**, а не гипотеза симуляции: утверждение состоит в том, что физика *есть* локальное унитарное правило, а не в том, что кто-то её *вычисляет*. Нет «до правила» и нет «снаружи правила» — есть только правило.

2. **Не «теория всего».** Подход классифицирует то, что выводимо из локальной унитарности, и то, что должно быть задано как вход. Он не выводит Стандартную модель, гравитацию или космологию. Восемь секторов класса A, четыре проверки класса B, пять отрицательных контролей класса C и **четыре** классификации данных — это **полный объём** работы, не больше.

3. **Не утверждение, что субстрат напрямую познаваем.** Мы видим «выход» (физику) и классифицируем его на структуру и данные. Мы не видим «железо». Существует ли железо, что оно собой представляет и как наш выход с ним соотносится — эти вопросы подход **оставляет в скобках**, а не решает. Классификация структура/данные работает *внутри* выхода, независимо от того, что за ним.

## Основные результаты

| Сектор | Эмерджентен? | Точность | Ноутбук |
|---|---|---|---|
| 1D Дирак | ✅ | 10⁻¹⁵ | 01 |
| U(1) калибровочное поле (фотон) | ✅ | 10⁻¹⁷ | 02 |
| SU(2) калибровочное поле (W/Z) | ✅ | 10⁻¹⁶ | 03 |
| Масса vs структура | ✅ | 10⁻¹⁶ | 04 |
| Хиггс (BCS-конденсат) | ✅ | 0.1% | 05 |
| 2D Дирак (сотовая решётка) | ✅ | α = 1.01, изотропия 1.0000 | 06 |
| 2D квадратная (контраст) | ❌ | отношение > 1.15 | 07 |
| 3D Дирак на 4D-стенке | ✅ | E₀ = 0, вес стенки 51%, изотропия 1.0 | 08 |
| SVD масс кварков | данные | ранг-1 (99.7%), фактор 2 | 09 |
| Скан баз (лептоны) | поисковое (не установлено) | база 15: dev = 0.028148; p_abs = 10/84 = 0.1190 | 10 |
| Геометрия 4D-стенки | ❌ (нулевой) | нет 1/32 в v_F или c | 11 |
| Частица–античастица | ✅ (структура) | m = m̄, CPT | 12 |
| Скан баз (нейтрино) | данные (частично) | Σmν = 0.0608 эВ (согласуется с DESI) | 13 |
| Фундаментальные константы | ❌ (данные) | нет скрытой сетки | 14 |
| Скорость света | ✅ (структура) | c = 1 (эмерджентно из локальности) | 15 |
| Квантовая запутанность | ✅ (структура) | CHSH = 2√2, C = 1 (сохраняется) | 16 |
| Принцип Паули | ✅ (структура) | Обмен = -1 (фермионы), +1 (бозоны) | 17 |
| 3 поколения | ✅ (структура) | N стенок → N мод (точно); 2D через фермионы перекрытия | 18 |
| CP-нарушение | ❌ (данные) | J(δ) — синусоида; фаза — вход | 19 |

**Главное:**

- **Структура** (калибровочные поля, Дирак, Хиггс, CPT, скорость света, запутанность, Паули, 3 поколения) — эмерджентна из QCA с машинной точностью.
- **Параметры** (массы, юкавские связи, константы, CP-фаза) — данные: несжимаемы, не рациональны, без естественной единицы.
- **Поисковое наблюдение (не установлено):** предпочтение базы 15 для лептонов. dev = 0.028148, p_abs = 10/84 = 0.1190 (выбор лучшего из 39). Статус: **не установлено** (дефицит до наводящего порога 5/84 = 0.0595). Кварки: MC-среднее на базе 40 = 0.178335; детерминированный dev_best39 = 0.174249; ни одна база не ниже 5%. Коэффициент эффекта поиска в другом месте = 4.76 (тройка {μ,b,t} на базе 40 лучше лептонов в 4.76 раза). Подход **не зависит** от базы 15.

## Классификация (19 ноутбуков)

Подход опирается на:

- **8 независимых выводов структуры** (класс A): nb01–06, nb08, nb18 Parts B–C;
- **4 проверки согласованности с квантовой механикой** (класс B): nb12, nb15–17;
- **5 отрицательных контролей** (класс C): nb07, nb11, nb14, nb18 Part A, nb19 T0–T2;
- **4 классификации данных** (данные): nb09 (SVD кварков), nb10 (скан баз), nb13 (нейтрино), nb19 T4–T5 (CP-фаза).

*Счётчики не пересекаются; отрицательные контроли не входят в число уровней подтверждения. nb18 разделён: Part A — класс C, Parts B–C — класс A. nb19 разделён: T0–T2 — класс C, T4–T5 — данные.*

## Текущий статус

### Ноутбук 10 — Скан баз: ПОИСКОВОЕ (не установлено)

Статистика: попарные логарифмические отношения `m_j/m_i` (инвариантна к масштабу по построению). База 15: dev = **0.028148 ± 1.6059×10⁻⁵** для лептонов. Пермутационный тест с выбором лучшего из 39: p_abs = **10/84 = 0.1190**, ранг лептонов = 10/84. Статус: **не установлено** (наводящий порог 5/84 = 0.0595).

Кварки: MC-среднее на базе 40 = **0.178335 ± 1.4605×10⁻²**; детерминированный dev_best39 = **0.174249**; 0 баз ниже 5%. Эффект поиска в другом месте: тройка {μ,b,t} на базе 40 даёт dev = 0.005912, в 4.76 раза лучше лептонов.

Фиксированная база 15 (вторичная строка, оговорка об апостериорном отборе): p_fixed = 1/84 = 0.0119. **Аннулирован апостериорным отбором** (база 15 найдена сканом по этим же данным). В аннотации и нижней строке выводов не используется.

2.8% и Койде (K = 2/3) не независимы: целые экспоненты дают K = 0.65591603, дробные части дают K = 0.66666378. Одно свидетельство в двух формулировках.

**Источник:** `nb10_pvalue_results.txt` (единственный источник всех чисел выше). **Рисунок:** `figures/10_base_scan.png`.

### Ноутбук 18 — Три поколения: ✅ ЗАКРЫТ (Структура)

N стенок → N мод точно в 1D SSH; 2D реализовано через фермионы перекрытия (остаток Гинзпарга–Вильсона ~3×10⁻¹⁵). Механизм = структура. Число N = 3 — вход.

**Рисунки:** `figures/18_partA_doubling.png`, `figures/18_partA_chiral.png`, `figures/18_partB_ssh.png`.

### Ноутбук 19 — CP-нарушение: ✅ ЗАКРЫТ (Данные)

T0–T2: CP сохраняется (1D, 2 поколения) — класс C, отрицательный контроль. T4: J(δ) ≠ 0 (3 поколения, toy CKM). T5: майорановский инвариант ≠ 0 (актуален только для 0νββ, не для осцилляций). Фаза δ — вход. **CP-нарушение = данные (4-я классификация данных).**

**Рисунок:** `figures/19_cp_violation.png`.

## Ограничения

1. QCA — подход, не «теория всего».
2. Все успешные результаты воспроизводят известную физику. Новых предсказаний не делается; Σmν = 0.0608 эВ (nb13) — **проверка согласованности** с верхним пределом DESI DR2, а не предсказание.
3. Юкавские связи не объяснены.
4. Интерпретация «4D-оператора» — философская.
5. **База 15 для лептонов — поисковая: p_abs = 10/84 = 0.1190, не установлено.** Коэффициент эффекта поиска в другом месте 4.76. Не поддерживает центральный тезис подхода.
6. Нейтрино и константы не следуют сетке базы 15.
7. 3 поколения: механизм точен в 1D; 2D требует фермионов перекрытия. Число N = 3 — вход.
8. CP-нарушение: подход может его вместить, но фаза δ — вход.
9. 2.8% отклонения базы 15 и Койде K = 2/3 не независимы (дробные экспоненты — следствие условия K = 2/3).
10. **Коэффициент эффекта поиска в другом месте 4.76 — нижняя граница поправки на множественность.** Он учитывает только 39 баз в nb10, но не гипотезы, проверявшиеся в v1–v13 (Койде, SVD, DESI, альтернативные нормировки). Реальная поправка на множественность строго больше 4.76, следовательно **p_abs = 0.1190 — нижняя граница, а не полная поправка**. Это делает вывод о базе 15 ещё менее установленным, а не более.
11. Проверки на устойчивость (зерно, N_MC, усреднение против максимума) в v14.4 не выполнены; план — в `nb10_pvalue.md` §6. Включение в v15.
12. **Многоцентровая космология не тестируется.** Подход нейтрален к начальным условиям: он не различает одноцентровую и многоцентровую инициализацию. Предварительные численные тесты (вне этой статьи) не показывают значимого сигнала; результат остаётся поисковым и не входит в статью.
13. **Космология отскока и предынфляционные фазы не тестируются.** Подход не предсказывает начальные условия; они классифицируются как «данные». Модели типа ekpyrotic/отскока совместимы с подходом, но не проверяются в нём.
14. **Гравитация не тестируется.** Эмерджентность 1/r² из QCA-решётки — задача отдельного ноутбука (nb20, запланирован), а не v14.4. Подход не претендует на вывод ОТО, принципа эквивалентности или квантовой гравитации.
15. **Киральные левые дублеты Стандартной модели не реализованы.** Фермионы перекрытия (nb18 Part C) дают технологию для точной киральной симметрии, но конкретное вложение SU(2)_L дублетов в QCA не выполнено. Это направление для v15+.

## Критерий фальсификации

Тезис «структура и данные» будет опровергнут, если:

1. Для кварков найдётся статистически значимая база (тем же методом; p < 0.01);
2. Добавление локальных унитарных взаимодействий (а) меняет классификацию какого-либо сектора с «структура» на «данные», или (б) требует подгонки параметра, ранее воспроизводившегося без неё;
3. CP-фаза будет выведена из QCA-правил без свободных параметров.

Ни одно из трёх не реализовалось. База 15 для лептонов **не проходит** критерий (i) при p < 0.01 — её p_abs = 0.1190 далеко от порога. Это согласуется с подходом: база 15 была поисковым наблюдением, а не структурным выводом.

## Структура репозитория

```text
qca-structure-data/
│
├── README.md                          # Этот файл (v14.4, EN + RU)
├── CHANGELOG.md                       # Трассировка R3–R18
├── nb10_pvalue.md                     # Пре-регистрация (зафиксирована до прогона)
├── nb10_pvalue_results.txt            # Фактический вывод прогона (единый источник)
├── LICENSE                            # MIT
├── requirements.txt
│
├── notebooks/
│   ├── 01..17_*.ipynb
│   ├── 18_three_generations.ipynb
│   └── 19_cp_violation.ipynb
│
├── data/
│   ├── quark_masses.csv
│   └── lepton_masses.csv
│
└── figures/
    ├── 01..17_*.png
    ├── 10_base_scan.png
    ├── 18_partA_doubling.png
    ├── 18_partA_chiral.png
    ├── 18_partB_ssh.png
    └── 19_cp_violation.png
```

## Требования

- Python 3.10+
- numpy 1.26.4, scipy 1.11.4, matplotlib 3.8.4

## Статус

- ✅ Ноутбуки 01–19 протестированы; результаты воспроизводятся с заявленной точностью
- ✅ База 15: финальный пермутационный тест завершён (p_abs = 10/84, НЕ установлено)
- ⏳ DOI Zenodo: готов к присвоению после коммита v14.4

## Лицензия

- **Код**: MIT
- **Текст и рисунки**: CC BY 4.0