# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?

> ./group_vars/*****/examp.yml  

2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?

> ansible-playbook **-i inventory/test.yml** site.yml  

3. Какой командой можно зашифровать файл?

> ansible-vault **encrypt** group_vars/{deb,el}/examp.yml

4. Какой командой можно расшифровать файл?

> ansible-vault **decrypt** group_vars/{deb,el}/examp.yml

5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?

> ansible-vault **edit** group_vars/deb/examp.yml

6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?

> ansible-playbook **--ask-vault-pass** -i inventory/prod.yml site.yml

7. Как называется модуль подключения к host на windows?

> **winrm**

8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh

> ansible-doc -t connection ssh

9. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?

> **remote_user**

