# IQMeter trap puzzles: how people answer in an online IQ test

Aggregated answer data from the [IQMeter](https://iqmeter.cloud) online IQ test, snapshot of **9 November 2026**:
**3,696 completed tests, 147,902 answers**, automated runs (bots) excluded. No personal data.

The headline: six classic puzzles that only **16–24%** of test-takers solved. In four of them, more than half of those who missed chose the same wrong answer. Try them and read the explanations: [iqmeter.cloud/en/traps/](https://iqmeter.cloud/en/traps/) · [на русском](https://iqmeter.cloud/ru/traps/).

| Puzzle | Answered | Correct | Most common wrong answer |
|---|---|---|---|
| Snail climbs 3 m by day, slides 2 m at night, 10 m well. Days? (8) | 609 | 16% | “10” — 51% |
| Angle between clock hands at 3:15 (7.5°) | 630 | 20% | “0°” — 42% |
| 2, 3, 5, 7, 11, 13, ? (17) | 829 | 24% | “15” — 52% |
| 5ˣ = 25³, find x (6) | 628 | 22% | “15” — 47% |
| Lie detector, 95% accurate, 10% liars. P(liar \| flagged)? (≈68%) | 613 | 16% | “≈95%” — 36% |
| Knight or knave says “I am a liar” (impossible) | 602 | 24% | “Knight” — 31% |

## Files

- `data/trap_puzzles.csv` — the six puzzles: question and options in Russian and English, number and share of answers for every option. `option_position = -1` means the person ran out of time.
- `data/categories.csv` — all questions grouped by category and difficulty (1 easy, 2 medium, 3 hard): number of questions, answers, share correct, share who ran out of time. Groups with fewer than 100 answers are not published. Question texts and answer keys of the live test are not included.
- `datapackage.json` — field descriptions (Frictionless Data Package).

## Method and limits

- Source: answers stored when a test is completed. Tests are excluded if the user agent is empty, matches a bot pattern, or belongs to seeded demo history.
- Participants are visitors to iqmeter.cloud: 63% from Kazakhstan, then Uzbekistan (6%), Ukraine (5%), Turkey (3%); 85 countries in total. Test languages: Kazakh 45%, Russian 39%, English 7%. **This is not a sample of any population**: the numbers describe how hard the puzzles are for this audience, not how intelligent any group is.
- Puzzles are solved inside a timed IQ test; each test shows 40 questions from a pool of about 600, so each question is answered by a subset of test-takers.
- Margin of error for the six puzzles is about ±3 percentage points.
- The six puzzles stay in the live test pool. Numbers are frozen at the snapshot date, because answers published here could bias later answers.
- `memory` is a new category with few answers. Some visual questions were redrawn in October 2026; their earlier answers may reflect the old images.

## License and citation

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Please credit “IQMeter (iqmeter.cloud)” with a link. Citation details are in `CITATION.cff`.

Mirrors: [GitHub](https://github.com/ChPuK/iqmeter-open-data) · [Hugging Face](https://huggingface.co/datasets/ChPuK/iqmeter-traps).

Contact: support@iqmeter.cloud

---

## Кратко на русском

Агрегированные ответы в онлайн-тесте IQ [IQMeter](https://iqmeter.cloud) на 9 ноября 2026 года: 3 696 завершённых тестов, 147 902 ответа, боты исключены, персональных данных нет. Шесть классических задач, которые решили только 16–24% участников, и сводка по всем категориям и уровням сложности. Задачи с разбором: [iqmeter.cloud/ru/traps/](https://iqmeter.cloud/ru/traps/).

Участники — посетители сайта (больше всего из Казахстана), это не выборка населения: цифры говорят о трудности задач, а не об уровне людей. Лицензия CC BY 4.0 — используйте со ссылкой на IQMeter.
