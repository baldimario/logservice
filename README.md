sudo mkdir /var/log/logservice
sudo mkdir /var/log/logservice/logs
sudo touch /var/log/chat_ids
sudo mkdir /etc/logservice
sudo cp -r ./dist/* /etc/logservice/
sudo cp ./logservice.service /etc/systemd/system/logservice.service
sudo systemctl daemon-reload
sudo systemctl enable logservice.service
sudo systemctl start logservice.service

