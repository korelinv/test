Релизовать формы просмотра и редактирования карточки

Сдалать возможным переиспользование полей для создания других форм

Модель данных

``` javascript
  
  {
      firstname: 'Иван',
      lastname: 'Иванов',
      patronymic: 'Иванович',
      countryId: 1,
      comment: null
  }

```

# Форма просмотра
поля:
- фио
- страна
- коментарий

поле фио является составным из полей имя фамилия и отчество (пример {firstname: 'Иван'. lastname: 'Иванов', patronymic: 'Иванович'} => 'Иванов И.И.')

поле коментарий не отображается если коментарий отсутсвует

кнопки:

- сохранить

при нажатии полей должна происходить валидация полей

если валидация не пройдена под незаполненными обязательными полями вывести 'Поле является обязательным для сохранения'

# Форма редактирования

поля ввода:
- имя (текстовое)
- фамилия (текстовое)
- отчество (текстовое)
- страна (выпадающий список)
- коментарий (текстовое)

поля имя, фамилия и страна являются обязательными

в выпадающем списке 'страна' Россия всегда должна отображаться первой в списке

данные для поля страна
    
``` javascript
  [
      {
          id: 1,
          name: 'Россия'
      },       
      {
          id: 4,
          name: 'КНР'
      },   
      {
          id: 2,
          name: 'Франция'
      },
  ]
```
