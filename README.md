# Pi-Baby-Monitor

# Source: https://github.com/iizukanao/picam

# Parts:
- Raspberry Pi 3 $40
- Night Vision For Raspberry Pi 3 with Infrared LED Lights (https://www.amazon.com/gp/product/B01ICLLOZ8/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1) $30
- Clip-on mic (https://www.amazon.com/gp/product/B01CRB67W4/ref=ox_sc_act_title_2?ie=UTF8&psc=1&smid=ATHX4IJBFO86X) $7
- Sound card adapter (https://www.amazon.com/gp/product/B00M3UWE3Q/ref=ox_sc_act_title_1?ie=UTF8&psc=1&smid=A2EQ48GCAFFFSI) $6
- Wall mount Brackets (https://www.amazon.com/gp/product/B00836ODGU/ref=oh_aui_detailpage_o07_s00?ie=UTF8&psc=1) $10

# Commands to start network monitor:

- sudo /usr/local/nginx/sbin/nginx
- ./picam -o /run/shm/hls
- ffmpeg -i index.m3u8 -c copy -bsf:a aac_adtstoasc -f flv rtmp://192.168.X.X/webcam/mystream
