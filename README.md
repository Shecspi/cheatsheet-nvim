# Шпаргалка по NeoVim

## Установка
0. Подготовка к установке
    - Установить специальных шрифтов Nerd Fonts. Их необходимо скачать с сайта https://www.nerdfonts.com/font-downloads и поместить в папку `~/.fonts`. После этого выполнить команду  
    ```bash
    fc-cache -v
    ```  
    - Установить [ripgrep](https://github.com/BurntSushi/ripgrep)  
   ```bash
   sudo pacman -S ripgrep
   ```  
    - Установить [lazygit](https://github.com/jesseduffield/lazygit)  
    ```bash
    sudo pacman -S lazygit
    ```
1. Удалить старую конфигурацию  
```bash
rm -rf ~/.config/nvim ~/.local/share/nvim ~/.cache/nvim ~/.local/state/nvim
```
2. Установить NeoVim  
```bash
sudo pacman -S neovim
```
3. Загрузить конфигурацию AstroNVim  
```bash
git clone --depth 1 https://github.com/AstroNvim/AstroNvim ~/.config/nvim
```
4. Запустить nvim и дождаться установки всех плагинов.  
```bash
nvim
```
5. Установить поддержку Python  
```
:LspInstall pyright
:TSInstall python
```

## Горячие клавиши
**Перемещение по тексту**  
`h` Влево  
`j` Вниз  
`k` Вверх  
`l` Вправо  

`w` Вперед на первую букву слова  
`e` Вперед на последнюю букву слова  
`b` Назад на первую букву слова  
`ge` Назад на последнюю букву слова

`0` На начало строки
`^` На первый не пустой символ строки
`$` На конец строки
`{` На абзац назад до пустой строки
`}` на абзац вперёд до пустой строки

`gg` В начало файла
`G` В конец файла
`Ctrl + u` На полэкрана вверх
`Ctrl + d` На полэкрана вниз

`>>` Сдвинуть строку вправо
`<<` Сдвинуть строку влево
