# Средство обнаружения вторжений Suricata и легковестный веб-интерфейс EveBox

В составе сборки: suricata -- сама IPS/IDS, evebox -- веб-морда для неё. 
Порт для доступа к веб-интерфейсу: 5636
```
suricta-main/          # Корневая директория
│
├── rules/             # Директория с правилами для обнаружения. Примонтирована к контейнеру Suricata.
│   └── <файлы_правил>
│
├── logs/              # Директория с логами
│   └──  <логи>
│
├── docker-compose.yml # Файл конфигурации для запуска всего кластера
└── suricata.yaml      # Файл конфигурации IPS/IDS Suricata
```
# TODO
- [x] Заменить правила на свежие англоязычные. (Пока на португальском, обновлю позже.)
- [ ] Докрутить сборку и правила до автоматической обороны от атак
