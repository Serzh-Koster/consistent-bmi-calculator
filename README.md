# Consistent BMI Calculator / Куркулятор CBMI

A bilingual, privacy-preserving, single-file calculator that compares three anthropometric models:

- experimental **CBMI**;
- conventional **BMI**;
- **waist-to-height ratio**.

Двомовний автономний куркулятор, який порівнює три антропометричні моделі:

- експериментальний **CBMI**;
- класичний **ІМТ**;
- **співвідношення талії до зросту**.

## Live site / Живий сайт

https://serzh-koster.github.io/consistent-bmi-calculator/

## What it does / Що він робить

The calculator:

- calculates CBMI, conventional BMI, and waist-to-height ratio;
- shows each result on a visual scale;
- compares whether the models converge or diverge;
- estimates the experimental CBMI weight range for the entered height;
- works in Ukrainian and English;
- runs entirely in the browser;
- does not send or store entered data.

Куркулятор:

- обчислює CBMI, класичний ІМТ і співвідношення талії до зросту;
- показує кожен результат на візуальній шкалі;
- дає змогу побачити сходження або розходження моделей;
- розраховує експериментальний діапазон маси для введеного зросту;
- працює українською та англійською;
- виконує всі обчислення безпосередньо у браузері;
- не передає й не зберігає введені дані.

## Formulas / Формули

### Experimental CBMI

```text
CBMI = √(mass / height³)
CBMI × 10 = 10 × √(mass / height³)
```

### Conventional BMI

```text
BMI = mass / height²
```

### Waist-to-height ratio

```text
WHtR = waist circumference / height
```

Mass is entered in kilograms, height in metres for CBMI and BMI, and waist and height in the same units for WHtR.

Маса вводиться в кілограмах, зріст для CBMI та ІМТ — у метрах, а талія і зріст для співвідношення талії до зросту — в однакових одиницях.

## Experimental CBMI ranges / Експериментальні діапазони CBMI

The interface uses the preliminary `CBMI × 10` ranges proposed in the 2026 study:

| CBMI × 10 | Interface label |
|---:|---|
| `< 33` | below research range |
| `33–<39` | within research range |
| `39–<45` | above research range |
| `45–<51` | high |
| `≥ 51` | very high |

Інтерфейс використовує попередні діапазони `CBMI × 10`, запропоновані в дослідженні 2026 року:

| CBMI × 10 | Назва в інтерфейсі |
|---:|---|
| `< 33` | нижче дослідницького діапазону |
| `33–<39` | у межах дослідницького діапазону |
| `39–<45` | вище дослідницького діапазону |
| `45–<51` | високий показник |
| `≥ 51` | дуже високий показник |

## Important limitation / Важлива межа

This project is an educational and exploratory tool. It does **not** provide a diagnosis, determine an “ideal weight,” or replace professional medical assessment.

CBMI is an experimental model based on a limited study sample. Its thresholds are preliminary and require broader independent validation. BMI, CBMI, and waist-to-height ratio do not fully account for muscle mass, body-fat distribution, oedema, spinal deformity, pregnancy, amputations, or other individual conditions.

Цей проєкт є пізнавальним і дослідницьким інструментом. Він **не** ставить діагноз, не визначає «ідеальну вагу» і не замінює професійної медичної оцінки.

CBMI є експериментальною моделлю, побудованою на обмеженій вибірці. Її пороги попередні й потребують ширшої незалежної перевірки. ІМТ, CBMI та співвідношення талії до зросту не враховують повністю м’язову масу, розподіл жирової тканини, набряки, деформації хребта, вагітність, ампутації та інші індивідуальні стани.

## Primary source / Основне джерело

Serdar Beji, Nezihe Kizilkaya Beji, Ümmü Mutlu. **Development of a Consistent Body Mass Index.** *Scientific Reports*, 2026.

DOI: https://doi.org/10.1038/s41598-026-61284-1

## Technical structure / Технічна будова

The entire project is contained in one file:

```text
index.html
```

It includes HTML, CSS, JavaScript, bilingual interface text, responsive desktop/mobile layouts, calculations, validation, and built-in boundary checks.

Увесь проєкт міститься в одному файлі:

```text
index.html
```

У ньому зібрані HTML, CSS, JavaScript, двомовний інтерфейс, адаптивні режими для комп’ютера й телефона, формули, перевірка введення та контроль граничних значень.

## Local use / Локальний запуск

Download `index.html` and open it in any modern browser. No server, build step, package manager, or external dependency is required.

Завантажте `index.html` і відкрийте його у сучасному браузері. Сервер, збирання, пакетний менеджер або зовнішні залежності не потрібні.

## Author / Автор

Developed by [Serhii Kosternyi](https://www.facebook.com/Kosterny/) in collaboration with **#Слідошіт** using ChatGPT.

Куркулятор розроблено [Сергієм Костерним](https://www.facebook.com/Kosterny/) у спільній взаємодії зі **#Слідошітом** у ChatGPT.

## License / Ліцензія

Released under the [MIT License](LICENSE).

Поширюється за умовами [MIT License](LICENSE).
