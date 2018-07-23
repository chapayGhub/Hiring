# Synesis sport: Senior Frontend developer


[Послать резюме](mailto:jobs+js.ems@synesis.ru?subject=Мне интересна Ваша вакансия: Senior Frontend разработчик)


```typescript
import { Component, OnInit } from '@angular/core';

export interface HR {
  email: string;
  skype: string;
  advancedLink: string;
}

export interface Vacancy {
  project: string;
  mainTechnology: string;
  useStyleGuide: boolean;
  useMergeRequest: boolean;
  isOutsource: boolean;
}

@Component({
    selector: "eg-vacancy",
})
export class VacancyComponent implements OnInit {

    public hr: HR = {
      email: "jobs+js.ems@synesis.ru",
      skype: "evgeniya.litvinhik777",
      advancedLink: "https://goo.gl/TWPxNm",
    };

    public vacancy: Vacancy = {
      project: "Event Management System",
      mainTechnology: "Angular 6",
      useStyleGuide: true,
      useMergeRequest: true,
      isOutsource: false,
    };

    public bonuses: string[] = [
      "Отличная зарплата",
      "MacBook Pro",
      "Отличный офис в центре города"
    ];

    private get description(): string {
      return `
        Задача: реализация собственного проекта на современных технологиях ${this.vacancy.mainTechnology}.
        Наши преимущества:
          новый собственный продукт, стартовавший в марте 2018; результаты увидим уже в 2019 году;
          жесткий подход к стайл гайду, пишем тесты;
          большая опытная команда с бородатым тим лидом во главе: делимся знаниями, пиццей, пивом;
          железо - MacBook;
          комфортный офис в стиле лофт в центре (кабинетная система), свой ресторан на первом этаже,
          беседка для тимбилдигов с личным мангальщиком и прочие плюшки.
        А теперь серьезно.
        Пишем информационную систему (Event Management System) c инфраструктурой для проведения крупных мероприятий
        как локального, так и международного уровня.
        Первый обкат продукта будет проходить на Европейских играх 2019 года в Минске.
        После всего сказанного вам просто необходимо узнать больше: ${this.hr.advancedLink}.
      `;
    }
}


```