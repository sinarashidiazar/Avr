# AVR Project - Calculator & Game 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Language](https://img.shields.io/badge/Language-C%2B%2B-blue.svg)](https://isocpp.org/)
[![Platform](https://img.shields.io/badge/Platform-AVR-green.svg)](https://www.microchip.com/en-us/products/microcontrollers-and-microprocessors/8-bit-mcus/avr-mcus)

---

## English 

This project contains two programs for AVR microcontrollers:

### 📁 Project Files

#### 1. Calculator.cpp
A complete calculator with the following features:
- Basic math operations: addition, subtraction, multiplication, division
- 7-segment display with 8 digits
- 16-button keypad
- Support for numbers up to 8 digits
- Clear button functionality

#### 2. Game.cpp
A simple game with the following features:
- Movement control with two buttons
- 16x8 LED matrix display
- Random obstacle generation system
- Increasing game speed over time

### 🔧 Required Hardware

- AVR Microcontroller (ATmega32 or similar)
- 7-segment display (8 digits)
- 4x4 keypad
- 16x8 LED matrix (for game)
- Pull-up resistors
- 1MHz crystal

### 📋 Hardware Connections

#### For Calculator:
- Port A: Keypad input (first 8 bits)
- Port B: Keypad input (second 8 bits)
- Port C: Display digit selection
- Port D: 7-segment display data

#### For Game:
- Port A: LED matrix data
- Port B: Row selection (first 8 bits)
- Port C: Row selection (second 8 bits)
- Port D: Control button input

### 🚀 Compilation and Execution

1. Install AVR-GCC and related tools
2. Compile files:
   ```bash
   avr-gcc -mmcu=atmega32 -Os -o calculator.elf Calculator.cpp
   avr-gcc -mmcu=atmega32 -Os -o game.elf Game.cpp
   ```
3. Convert to hex file:
   ```bash
   avr-objcopy -O ihex calculator.elf calculator.hex
   avr-objcopy -O ihex game.elf game.hex
   ```
4. Upload to microcontroller using appropriate programmer

### 📝 Code Description

#### Calculator:
- Uses multiplexing for multi-digit display
- Button press detection with debouncing
- Math operation management and result display

#### Game:
- Uses timer for speed control
- Random obstacle generation
- Collision detection and game over

---

## فارسی

این پروژه شامل دو برنامه برای میکروکنترلر AVR است:

### 📁 فایل‌های پروژه

#### 1. Calculator.cpp
یک ماشین حساب کامل با قابلیت‌های زیر:
- عملیات ریاضی پایه: جمع، تفریق، ضرب، تقسیم
- صفحه نمایش 7-segment با 8 رقم
- کیبورد 16 دکمه‌ای
- پشتیبانی از اعداد تا 8 رقم
- دکمه پاک کردن (Clear)

#### 2. Game.cpp
یک بازی ساده با قابلیت‌های زیر:
- کنترل حرکت با دو دکمه
- نمایش LED ماتریسی 16x8
- سیستم تصادفی برای تولید موانع
- افزایش سرعت بازی با گذشت زمان

### 🔧 سخت‌افزار مورد نیاز

- میکروکنترلر AVR (ATmega32 یا مشابه)
- صفحه نمایش 7-segment (8 رقم)
- کیبورد 4x4
- LED ماتریس 16x8 (برای بازی)
- مقاومت‌های pull-up
- کریستال 1MHz

### 📋 اتصالات سخت‌افزاری

#### برای ماشین حساب:
- پورت A: ورودی کیبورد (8 بیت اول)
- پورت B: ورودی کیبورد (8 بیت دوم)
- پورت C: انتخاب رقم نمایش
- پورت D: داده‌های نمایش 7-segment

#### برای بازی:
- پورت A: داده‌های LED ماتریس
- پورت B: انتخاب ردیف (8 بیت اول)
- پورت C: انتخاب ردیف (8 بیت دوم)
- پورت D: ورودی دکمه‌های کنترل

### 🚀 نحوه کامپایل و اجرا

1. نصب AVR-GCC و ابزارهای مربوطه
2. کامپایل فایل‌ها:
   ```bash
   avr-gcc -mmcu=atmega32 -Os -o calculator.elf Calculator.cpp
   avr-gcc -mmcu=atmega32 -Os -o game.elf Game.cpp
   ```
3. تبدیل به فایل hex:
   ```bash
   avr-objcopy -O ihex calculator.elf calculator.hex
   avr-objcopy -O ihex game.elf game.hex
   ```
4. آپلود روی میکروکنترلر با استفاده از programmer مناسب

### 📝 توضیحات کد

#### ماشین حساب:
- استفاده از multiplexing برای نمایش چندین رقم
- تشخیص فشار دکمه با debouncing
- مدیریت عملیات ریاضی و نمایش نتایج

#### بازی:
- استفاده از تایمر برای کنترل سرعت
- تولید تصادفی موانع
- تشخیص برخورد و پایان بازی

---

## 📄 License | لایسنس

This project is licensed under the MIT License. See the LICENSE file for more details.

این پروژه تحت لایسنس MIT منتشر شده است. برای جزئیات بیشتر فایل LICENSE را مطالعه کنید.

## 🤝 Contributing | مشارکت

To contribute to this project:
1. Fork the project
2. Make your changes
3. Submit a pull request

برای مشارکت در این پروژه:
1. پروژه را fork کنید
2. تغییرات خود را اعمال کنید
3. یک pull request ارسال کنید

## 📞 Contact | تماس

For questions and suggestions, please create a new issue in the repository.

برای سوالات و پیشنهادات، لطفاً issue جدیدی در repository ایجاد کنید.

---

**Note | نکته**: This project is designed for educational purposes and can be used as a foundation for more complex AVR projects.

این پروژه برای اهداف آموزشی طراحی شده است و می‌تواند به عنوان پایه‌ای برای پروژه‌های پیچیده‌تر AVR استفاده شود.

