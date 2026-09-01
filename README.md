# Ручные задания для курса «Алгоритмы и структуры данных» 📝

Задачи решаются **вручную и оформляются в формате Markdown**, без программного кода. Среда — [Visual Studio Code](https://code.visualstudio.com/). Виртуальное окружение Python здесь **не нужно**.

Инструкции курса (репозиторий [docs](https://github.com/hse-algo-ps-25-1/docs)):

- [Установка необходимого ПО](https://github.com/hse-algo-ps-25-1/docs/blob/main/%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0%20%D0%BD%D0%B5%D0%BE%D0%B1%D1%85%D0%BE%D0%B4%D0%B8%D0%BC%D0%BE%D0%B3%D0%BE%20%D0%9F%D0%9E.md) — GitHub, Git, VS Code, клонирование этого репозитория
- [Структура ветвления](https://github.com/hse-algo-ps-25-1/docs/blob/main/%D0%9E%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5%20%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%82%D1%83%D1%80%D1%8B%20%D0%B2%D0%B5%D1%82%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D1%8F%20%D1%80%D1%83%D1%87%D0%BD%D1%8B%D1%85%20%D0%B8%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BD%D1%8B%D1%85%20%D0%B7%D0%B0%D0%B4%D0%B0%D1%87.md) — чем ручные задания отличаются от программных

Программные задания — в отдельном репозитории [code-tasks](https://github.com/hse-algo-ps-25-1/code-tasks). Правила веток и pull request там **другие**.

## С чего начать

1. Настроить VS Code по инструкции по установке ПО и **клонировать этот репозиторий** (`manual-tasks`).
2. Для превью Markdown и диаграмм Ганта / сетей поставьте расширения [Markdown Preview Github Styling](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles) и [Markdown Preview Mermaid Support](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid).

Оформить решение: [руководство по Markdown](https://gist.github.com/Jekins/2bf2d0638163f1294637), формулы — [LaTeX](https://grammarware.net/text/syutkin/MathInLaTeX.pdf).

## Задания

Условия лежат в каталогах ветки `main`, например `Задание 3`. В каталоге — `README.md` с постановкой и правилами оформления.

Решение команды — файл `<название_команды>.md` **в том же каталоге** (не в корне репозитория). Что именно должно быть в файле (вариант, ход решения, диаграммы) — в README задания.

Для работы создайте ветку **от `main`**, например `first-team-task-3`. В `main` напрямую не коммитьте.

## Результат выполнения задания: pull request

Это не `code-tasks`: здесь pull request открывают **в `main`**, и после ревью его **вливают**.

- **base** — `main`, **compare** — ваша ветка (`first-team-task-3`).
- Замечания правят новым коммитом в ту же ветку, новый pull request создавать не нужно.
- После одобрения изменения попадают в `main`: там остаются и условия, и решения команд. Эти материалы можно использовать для подготовки к контрольным работам и экзаменам по дисциплине.
