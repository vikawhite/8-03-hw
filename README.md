**# Домашнее задание к занятию "`8-03`" - `Trunova Vika`**

<ins>## Задание 1 </ins>

Результаты приложены в скриншотах 1-6, в 6 представлена запись runner


![Скриншот 1](https://github.com/vikawhite/8-03-hw/blob/main/runner/1.png)
![Скриншот 2](https://github.com/vikawhite/8-03-hw/blob/main/runner/2.png)
![Скриншот 3](https://github.com/vikawhite/8-03-hw/blob/main/runner/3.png)
![Скриншот 4](https://github.com/vikawhite/8-03-hw/blob/main/runner/4.png)
![Скриншот 5](https://github.com/vikawhite/8-03-hw/blob/main/runner/5.png)
![Скриншот 6](https://github.com/vikawhite/8-03-hw/blob/main/runner/6.png)


---

<ins>## Задание 2 </ins>

#Содержание моего файла  gitlab-ci.yml

stages:
  - test
  - build

test:
  stage: test
  image: golang:1.17
  script: 
   - go test .

build:
  stage: build
  image: docker:latest
  script:
   - docker build .


![Скриншот 1](https://github.com/vikawhite/8-03-hw/blob/main/01.png)
![Скриншот 2](https://github.com/vikawhite/8-03-hw/blob/main/3.png)
![Скриншот 3](https://github.com/vikawhite/8-03-hw/blob/main/2.png)


---


