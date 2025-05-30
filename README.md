# Inno_diploma
# Применение графов знаний для построения рекомендательных систем в образовании

## Описание проекта
Данный проект направлен на решение проблемы несоответствия между навыками, формируемыми в системе высшего образования, и актуальными требованиями рынка труда. В рамках работы была разработана рекомендательная система, основанная на графах знаний, объединяющих данные из вакансий, онлайн-курсов и образовательной программы магистратуры университета Иннополис по направлению «Управление на основе данных».

## 📊 Цель
Разработка методологии, позволяющей эффективно анализировать связи между образовательными и профессиональными навыками с использованием графов знаний и рекомендательных систем. 


## 🧩 Используемые данные
1. **Вакансии** — парсинг с hh.ru
2. **Онлайн-курсы** — парснг с платформы OpenEdu
3. **Образовательная программа** — карта компетенций магистратуры Иннополис

## 🛠️ Pipeline работы
<img src="https://github.com/user-attachments/assets/e540a4ed-e898-4cc8-9fc8-251328d597c2" width="700"/>

1. **Сбор и предобработка данных**  
2. **Стандартизация терминов** (с помощью модели OpenAI GPT-5.0)
3. **Определение онтологии**
4. **Построение графов знаний для каждого источника данных**
5. **Интеграция трех графов знаний**
6. **Хранение и визуализация в Neo4j**
7. **Рекомендательная система на основе векторной, графовой и  гибридной близости**

## Онтология и граф знаний
Пример определенной онтологии для онлайн-курсов

<img src="https://github.com/user-attachments/assets/6d7987ec-694d-44c5-a440-4b6b1b605b76" width="500"/>

Пример графа знаний для онлайн-курса "Теория вероятностей и математическая статистика для инженеров"

<img src="https://github.com/user-attachments/assets/1b1426bb-367d-440a-9c40-ce965dafb0eb" width="400"/>

## 📈 Оценка полученных рекомендаций
<img src="https://github.com/user-attachments/assets/030a0a89-5d7b-4a0e-80fc-41fa0ab46fa8" width="500"/>

Используемые метрики:
- `Macro-Precision@N`:
- `Macro-Recall@N`: 
- Метрики ранжирования: `MRR@5`, `nDCG@5`, `AP@5`
- Доверительные интервалы на основе метода Bootstrap

## 📌 Потенциал дальнейшего развития
- Разработка более гибких методов стандартизации терминов
- Интеграция с другими платформами (Coursera, Stepik)
- Масштабирование (динамическое обновление графа, автоматический парсинг данных)
- Адаптивная персонализация
- Разработка визуального интерфейса для интерпретируемости рекомендательной системы
