# cdnfly-kaixin

主控


curl -fsSL https://github.com/Steady-WJ/cdnfly-kaixin/raw/main/master.sh -o master.sh && chmod +x master.sh && ./master.sh --es-dir /home/es


被控


curl -fsSL https://github.com/Steady-WJ/cdnfly-kaixin/raw/main/agent.sh -o agent.sh  && chmod +x agent.sh && ./agent.sh --master-ver v5.1.13 --master-ip  --es-ip  --es-pwd 



