# Golden Apple Gift

## Описание
Этот проект содержит зашифрованный URL, доступ к которому можно получить с помощью закрытого GPG-ключа. Закрытый ключ и пароль для него будут переданы получателю отдельно.

## Содержимое
- **`encripted_gift.gpg`** – зашифрованный URL.
- **`private_key.asc`** – закрытый GPG-ключ.

## Расшифровка

### 1. Установка GPG (если не установлено)
- **MacOS:**
  ```bash
  brew install gnupg
  ```

### 2. Импорт закрытого ключа
```bash
gpg --import private_key.asc
```

### 3. Расшифровка URL
```bash
gpg --decrypt encripted_gift.gpg
```

После выполнения команды GPG запросит пароль от закрытого ключа. Введите пароль, и зашифрованный URL будет отображён в консоли.

## Важно
- Никогда не публикуйте закрытый ключ и пароль вместе.
- Закрытый ключ защищён паролем. Если вы потеряете пароль, расшифровать данные будет невозможно.

## Контакт
Если возникли вопросы или требуется дополнительная информация, свяжитесь со мной по почте или через другой канал.

![Golden Apple Gift](github_logo.png)

