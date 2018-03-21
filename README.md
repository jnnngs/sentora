# sentora

#install git
sudo apt-get update
sudo apt-get install git

#harden ubuntu

https://github.com/konstruktoid/hardening
Login, set a Grub2 password, configure and run ubuntu.sh
Do not add any packages.
Log in.
Select a Grub2 password (using grub-mkpasswd-pbkdf2).
Download the script using git clone https://github.com/konstruktoid/hardening.git
Change the configuration options in the ubuntu.cfg file and last but not least run the script, sudo bash ubuntu.sh

#install sentora

bash <(curl -L -Ss http://sentora.org/install)

#fix session problem (located in CRON)


[ -x /usr/lib/php5/maxlifetime ] && [ -x /usr/lib/php5/sessionclean ] && [ -d /var/sentora/sessions ] && /usr/lib/php5/sessionclean /var/sentora/sessions $(/usr/lib/php5/maxlifetime)

#create backup script

git clone https://github.com/neggs/sentora/raw/master/backup.sh

#SSH Security Banner

https://rbgeek.wordpress.com/tag/ssh-warning-banner/

#install webmin

https://www.digitalocean.com/community/tutorials/how-to-install-webmin-on-ubuntu-16-04
