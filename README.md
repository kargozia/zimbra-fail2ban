# zimbra-fail2ban
curl -k https://raw.githubusercontent.com/kargozia/zimbra-fail2ban/main/sshd.local > /etc/fail2ban/jail.d/sshd.local
curl -k https://raw.githubusercontent.com/kargozia/zimbra-fail2ban/main/zimbra.local > /etc/fail2ban/jail.d/zimbra.local
curl -k https://raw.githubusercontent.com/kargozia/zimbra-fail2ban/main/zimbra-web.conf > /etc/fail2ban/filter.d/zimbra-web.conf
curl -k https://raw.githubusercontent.com/kargozia/zimbra-fail2ban/main/zimbra-smtp.conf > /etc/fail2ban/filter.d/zimbra-smtp.conf
systemctl restart fail2ban
systemctl status fail2ban
systemctl enable fail2ban
