This ansible script is an work in progress.
Please note, I use this repository for docker-container https://github.com/Andre-learnbox/ollama-open-webui

Additional you need an inventory file like this

[ollama_servers]
server1 ansible_host=192.168.1.100

[all:vars]
ollama_url=http://localhost:11434
ollama_port=11434
webui_url=http://localhost:3000
webui_port=3000
webui_domain=your_domain
ollama_domain=your domain
certbot_email=your-email@domain.com

ansible-playbook -i inventory.yml install_open-webui.yml
