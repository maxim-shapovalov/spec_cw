# Итоговая контрольная работа по блоку Специализация 5277

## Информация о проекте
Необходимо организовать систему учета для питомника в котором живут
домашние и вьючные животные.


## 1. Используя команду cat в терминале операционной системы Linux, создать
два файла Домашние животные (заполнив файл собаками, кошками,
хомяками) и Вьючные животными заполнив файл Лошадьми, верблюдами и
ослы), а затем объединить их. Переименовать файл, дав ему новое имя (Друзья человека). 
Просмотреть содержимое созданного файла. 

```sh
cat > Pets
dogs
cats
hamsters
```
```sh
cat > Pack_animals
horses
camels
donkeys
```
```sh
cat Pets Pack_animals > Human_Friends
```
```sh
cat Human_Friends
```
![commands](images/linux1.PNG)

## 2. Создать директорию, переместить файл туда. 

```sh
mkdir animals
```
```sh
mv Human_Friends animals
```
![commands](images/linux2.PNG)

## 3. Подключить дополнительный репозиторий MySQL. Установить любой пакет из этого репозитория.

```sh
apt update
apt install mysql-server
```
![install mysql](images/linux3.PNG)
![install mysql](images/linux3_1.PNG)

## 4. Установить и удалить deb-пакет с помощью dpkg.

```sh
wget https://dev.mysql.com/get/mysql-apt-config_0.8.25-1_all.deb
dpkg -i mysql-apt-config_0.8.25-1_all.deb
```

![download debpacket](images/linux3_3.PNG)
![install debpacket](images/linux3_2.PNG)

## 5. Выложить историю команд в терминале ubuntu

![command history](images/linux_history.PNG)

Идеальный набор команд выглядит так:
```sh
  574  cat > Pets
  575  cat Pets
  576  cat > Pack_animals
  577  cat Pack_animals
  578  cat Pets Pack_animals > Human_Friends
  579  cat Human_Friends
  580  mkdir animal
  581  mv Human_Friends animals
  582  ls animals
  583  sudo apt update
  584  sudo apt install mysql-server
  595  wget https://dev.mysql.com/get/mysql-apt-config_0.8.25-1_all.deb
  596  sudo dpkg -i mysql-apt-config_0.8.25-1_all.deb
```
