# Synesis sport: iOs developer


[Послать резюме](mailto:jobs+ios@synesis.ru?subject=Мне%20интересна%20Ваша%20вакансия:%20iOs%20разработчик)


```swift
//
//  iOs-position.swift
//  Synesis-sport
//
//  Created by Synesis-sport on 7/10/18.
//  Copyright © 2018 Synesis-sport. All rights reserved.
//

import Foundation

@available(iOS 10.0, *)
public class N​ew_Team_Member: Senior_iOs_Developer {
  /*
      В рамках нашей компании мы формируем мобильную
   команду для нового проекта и ​ ищем S​enior iOS
   ​разработчика для написания мессенджера, а также
   мобильных приложений разрабатываемых в рамках игр.
    Проект пишется с нуля с марта 2018.
    Работаем над созданием Информационной системы (Event
     Management System) c ​инфраструктурой для проведения
   крупных мероприятий как локального, так и международного
   уровня.
   */

  public static let требования: [String: Bool] = [
    "работы в команде iOS разработчиков": true,
    "разработка под iOs от 3 лет": true,
    "активной разработки на Swift от 1 года": true,
    "реализации REST API взаимодествия в iOS приложении": true,
    """
     опыт интеграции
    ​  - push notifications,
      - deeplinking,
      - аналитики и прочих мобильных плюшек
    """: true,
    """
     разработки iOS клиента самостоятельно
     (не обязательно именно свои проекты)
    """: true
  ]

  public static let п​риветствуются: [String] = [
    "понимание/опыт работы с MVVM, VIPER, RxSwift, ReactiveSwift, Realm и ...",
    "желание получать и делиться опытом с коллегами",
    "инициативность",
    "ответственность",
    "​здравая оценка своих возможностей"
  ]

  public static let задача = "создание качественного, расширяемого продукта в команде единомышленников"

  public static func readMore() {
    let subjectText = "subject=Мне интересна Ваша вакансия: iOs разработчик"
    guard
        let mailSubject = subjectText.addingPercentEncoding(withAllowedCharacters: .urlQueryAllowed),
        let url = URL(string: "mailto:jobs@synesis.ru?\(mailSubject)")
    else
        { return }

    UIApplication.shared.open(url, options: [:], completionHandler: nil)
  }
}
```