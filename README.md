# ArchLinux Fast Install
This script install ArchLinux XFCE + AUR + XFCE config. Also you can add own /home directory as well as XFCE config.

# Описание
Этот скрипт не задумывался, как обычный установочный с большим выбором DE, разметкой диска и т.д.

Его цель - это моментальное разворачиванеи системы со всеми конфигами. Смысл в том что, все изменения вы делаете предварительно в самом скрипте и получаете возможность быстрой установки ArchLinux XFCE + AUR + XFCE с вашими личными настройками (при условии, что вы его изменили под себя, в противном случае с моими настройками).

Cкрипт основан на моем чек листе ручной установке ArchLinux https://vk.cc/7JTg6U
Разметка MBR c BIOS. C UEFI пока установки нет. В планах.

Cостоит из 3 частей. 

Видео с демонстрацией работы скрипта https://www.youtube.com/watch?v=nvVF_qKDUeM

# Установка 
1) Скачать и записать на флешку ISO образ Arch Linux https://www.archlinux.org/download/
2) Скачать и запустить скрипт командой:

   ```bash 
   wget git.io/arch1.sh && sh arch1.sh
   ```
   Запустится установка минимальной системы с DE XFCE.
   2-я часть ставится автоматически и это базовая установка ArchLinux без программ. 
3) 3-я часть не обязательная. Она устанавливает программы, AUR (yay), мои конфиги XFCE.
   Предварительно установите wget командой:
   ```bash 
   sudo pacman -S wget
   ```
   Установка 3-й части производится из терминала командой:
   
   ```bash 
   wget git.io/arch3.sh && sh arch3.sh
   ```

# Настройка скрипта под себя
Вы можете форкнуть этот срипт. Изменить разметку дисков под свои нужды, сделать копию конфга XFCE, залить его на Github и производить быстрое разворачивание вашей системы.
По завершению работы скрипта вы получаете вашу готовую и настроенную систему со всеми конфигами. Вам ее нужно лишь немного привести в порядок и все.
Как и что менять написано в комментариях в самом скрипте.

# ВНИМАНИЕ!
Автор не несет ответственности за любое нанесение вреда при использовании скрипта. Используйте его на свой страх и риск или изменяйте под свои личные нужды.

Если вам не подходит автоматическая разметка дисков, тогда вам, предварительно нужно сделать разметку дисков и настроить скрипт под свои нужды (программы, XFCE config и т.д.)
Смотрите пометки в самом скрипте.

# Контакты
Наша группа по Arch Linux https://vk.com/arch4u

Linux Chat https://t.me/linux4u

# История изменений
18.03.2019 
- Теперь можно вводить собственное имя хоста и юзера
- Исправлен 3-й файл с установкой темой
- aurman заменен на yay
