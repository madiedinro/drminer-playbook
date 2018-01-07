Ansible playbook, чтобы развернуть на сервере Ubuntu майнер, который будет монетизировать свободные процессорные ресурсы. Майнит Monreo, где как раз не нужно GPU. 
Идеально для установки на серваках, где простаивает процессор.

# Запуск скрипты установки 


    ANSIBLE_HOST_KEY_CHECKING=false \
      ansible-playbook drminer.yml -i inventories/name
      
    
Опционально выполнить или исключить группы задач 

    --tags 'tag1,tag2'
    
или

    --skip-tags 'tag2,tag4'
    

