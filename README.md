# cdnfly-kaixin
仅支持CENTOS7
web目录为云端验证文件，请自行搭建

0.0.0.0改成(自己搭建的验证服务器Ip)
vi /etc/hosts

0.0.0.0  auth.cdnfly.cn

0.0.0.0  monitor.cdnfly.cn



v5.1.13主控


curl -fsSL https://github.com/Steady-WJ/cdnfly-kaixin/raw/main/master.sh -o master.sh && chmod +x master.sh && ./master.sh --es-dir /home/es


v5.1.16被控


curl -fsSL https://github.com/Steady-WJ/cdnfly-kaixin/raw/main/agent.sh -o agent.sh  && chmod +x agent.sh && ./agent.sh --master-ver v5.1.13 --master-ip  --es-ip  --es-pwd 



