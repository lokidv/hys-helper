first of all you need to update the server

```
sudo apt update && sudo apt upgrade -y
```
then you need to install marzneshin in the iran (main) server 

```
sudo bash -c "$(curl -sL https://github.com/marzneshin/Marzneshin/raw/master/script.sh)" @ install
```
if it doesn't work you need to set shecan dns in the server

```
nano /etc/resolv.conf
```
and then paste dns in there 

```
nameserver 178.22.122.100
nameserver 185.51.200.2
```
and save ctrl +c then enter and again paste installation command


for create login user
```
marzneshin cli admin create --sudo
```
for change port and path
```
nano /etc/opt/marzneshin/.env
```

change port and path
then
```
 marzneshin restart
```

so you need to make sub domain in cloudeflare and try to get ssl for that
```

آموزش گرفتن سرتیفیکیت برای مرزنشین ( acme.sh )


توجه : 

قسمت هایی ک YourDomain.com نوشته شده را دامین خودتونو قرار بدید.
1⃣

apt-get update

2⃣
apt install curl socat -y

3⃣

curl https://get.acme.sh | sh

4⃣

~/.acme.sh/acme.sh --set-default-ca --server letsencrypt

5⃣

~/.acme.sh/acme.sh --register-account -m daksaastuti.dw@gmail.com

6⃣

~/.acme.sh/acme.sh --issue -d hys1.inknobe.site --standalone

7⃣

mkdir -p /var/lib/marznode/certs

8⃣
~/.acme.sh/acme.sh --installcert -d hys1.inknobe.site --key-file /var/lib/marznode/certs/private.key --fullchain-file /var/lib/marznode/certs/cert.crt

```


in the foren server paste this command

```
sudo apt install unzip
bash <(curl -Ls https://raw.githubusercontent.com/mikeesierrah/ez-node/main/marznode.sh)
```

```
cd /opt/marznode/marz/hysteria
rm -f marz-teria

wget -O marz-teria https://github.com/apernet/hysteria/releases/download/app/v2.6.5/hysteria-linux-amd64
chmod +x marz-teria

./marz-teria version

```

then go to panel and setting then click in copy certificate
we neet if for config foren server



