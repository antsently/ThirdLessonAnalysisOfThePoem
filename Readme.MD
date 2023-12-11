## ThirdLessonAnalysisOfThePoem
```java
protected void onCreate(...) {
    ...

    // привязка разметки к полям
    output = findViewById(R.id.output);

    // конвертирование строки в массив и его сортировка
    poemArray = stringToArray(poem);
    Arrays.sort(poemArray);

    // вывод проанализированных данных на экран смартфона
    output.setText(Arrays.toString(poemArray));
}

    // остальные методы остаются без изменений

    // метод конвертирования строки в массив
private String[] stringToArray(String text) {
    String textMod = text.replaceAll("[^А-Яа-яёЁ]", " ").trim();
    return textMod.split("\\s+");
}
```
Исходник:

![Img](https://github.com/Antsently/ThirdLessonAnalysisOfThePoem/blob/master/img/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D0%B8%D0%BA.png?raw=true)


Доработанный вариант:

![Img](https://github.com/Antsently/ThirdLessonAnalysisOfThePoem/blob/master/img/%D1%80%D0%B5%D0%B4.png?raw=true)