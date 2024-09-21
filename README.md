# Devices

![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)
![Platform](https://img.shields.io/badge/platform-iOS%20%7C%20iPadOS-lightgrey.svg)

## Описание

**Devices** — это небольшой Swift-пакет для получения информации о модели устройства. Пакет позволяет легко получить модель текущего устройства и поддерживает множество моделей iPhone, iPad и iPod.

## Установка

### Swift Package Manager (SPM)

Для добавления пакета через Swift Package Manager в Xcode:

1. Перейдите в меню: **File > Add Packages...**
2. Введите URL репозитория: `https://github.com/yourusername/Devices.git`
3. Установите версию (например, `from: "1.0.0"`) и добавьте пакет в ваш проект.

Или добавьте вручную в ваш `Package.swift` файл:

```swift
dependencies: [
    .package(url: "https://github.com/lobanovD/Devices.git", from: "1.0.0")
]
```
## Использование
```swift
import Devices

let deviceModel = Devices.shared.deviceModel()
print("Модель устройства: \(deviceModel)")
```
## Поддерживаемые модели устройств
Пакет поддерживает следующие устройства:

- iPhone (начиная с iPhone 1-го поколения и до iPhone 15 Pro Max)
- iPod (до 7-го поколения)
- iPad (включая все поколения и модели iPad Air, iPad mini, iPad Pro)

## Лицензия
Этот проект лицензирован под лицензией MIT. См. файл LICENSE для подробной информации.
