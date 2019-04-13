# My Home Assistant Setup
<details>
<summary>
  <b>Compute & Detection</b></summary>
  <ul>
  <li><a href="https://www.intel.com/content/www/us/en/products/boards-kits/nuc/kits/nuc7i5bnh.html">Intel NUC</a></li>
  <li><a href="https://www.aliexpress.com/item/Wireless-Zigbee-CC2531-Sniffer-Bare-Board-Packet-Protocol-Analyzer-Module-USB-Interface-Dongle-Capture-Packet-Module/32852226435.html?spm=2114.search0104.3.9.6ae64da4Ihy5MO&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10902_10059_10884_10887_321_322_10103,searchweb201603_57,ppcSwitch_0&algo_expid=532ac65a-3e80-4722-aded-c42d3397f247-1&algo_pvid=532ac65a-3e80-4722-aded-c42d3397f247">CC 2531</a></li>
  </ul>
</details>
<details>
<summary>
  <b>Network</b></summary>
  <p><a href="https://store.google.com/product/google_wifi">Google Wi-Fi</a></p>
</details>
<details>
<summary>
  <b>Sensors</b></summary>
  <p>I like using Xiaomi sensors as they're cheap, reliable, and portable. This is especially relevant to my use case as I bought the majority of the sensors used in my setup as a renter. I'm in the process of building a house and these sensors will be quick to pack up and set-up in the new house. I don't trust the original Xioami gateway, which often phones home to China so I blocked internet access to the gateway, which acts as the Zigbee coordinator. Eventually, I'll remove the gateway altogether and just use Zigbee2mqtt as a bridge between each device and Home Assistant</p>
  <ul>
  <li><a href="https://www.aliexpress.com/item/New-Original-Xiaomi-Mijia-Human-Body-Sensor-Infrared-Smart-Home-Detector-Motion-Sensor-Safe-Moistureproof-15ms/32858852215.html?spm=2114.search0104.3.19.111f316b2zfoj2&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10902_10059_10884_10887_321_322_10103,searchweb201603_57,ppcSwitch_0&algo_expid=cfc297f2-d6a6-4952-a632-a63ac3f66fdd-2&algo_pvid=cfc297f2-d6a6-4952-a632-a63ac3f66fdd">Xiaomi Mijia Human Body Sensor</a></li>
  <li><a href="https://www.aliexpress.com/item/2019-Xiaomi-Mi-Smart-Temperature-and-Humidity-Sensor-Mini-Intelligent-Sensor-Put-the-baby-Home-office/32986664949.html?spm=2114.search0104.3.32.17e2205013KSAz&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10902_10059_10884_10887_321_322_10103,searchweb201603_57,ppcSwitch_0&algo_expid=246f6dd6-c260-492f-82da-5b9358ca0864-7&algo_pvid=246f6dd6-c260-492f-82da-5b9358ca0864">Xiaomi Mi Smart Temperature & Humidty</a></li>
  <li><a href="https://www.aliexpress.com/item/Xiaomi-Aqara-Wireless-Flood-Water-Immersing-Sensor-IP67-Waterproof-App-Remote-Cantrol-Remote-Mijia-Smart-Home/32921707280.html?spm=2114.search0104.3.55.69e2fec1u0Ht7A&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10902_10059_10884_10887_321_322_10103,searchweb201603_57,ppcSwitch_0&algo_expid=9c9b4499-285b-4f4c-9fee-6efad92b8e55-7&algo_pvid=9c9b4499-285b-4f4c-9fee-6efad92b8e55">Xiaomi Aqara Water Sensor</a></li>
  <li><a href="https://www.aliexpress.com/item/HOT-Original-Xiaomi-Door-Window-Sensor-Pocket-Size-Xiaomi-Smart-Home-Kits-Alarm-System-Work-with/32965692266.html?spm=2114.search0104.3.17.17c12c44nGAg85&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10902_10059_10884_10887_321_322_10103,searchweb201603_57,ppcSwitch_0&algo_expid=bfe0ecfe-0bb3-4e45-a9b7-678244bb4d78-2&algo_pvid=bfe0ecfe-0bb3-4e45-a9b7-678244bb4d78">Xiaomi Door/Window Sensor</a></li>
  </ul>
</details>
<details>
    <summary>
  <b>Software</b>  </summary>
    <p><strong>OS</strong></p><p><a href="http://releases.ubuntu.com/18.04/">Ubuntu 18.04 LTS</a></p>
  <p><strong>Docker Containers</strong></p> 
  <ul>
    <li><a href="https://hub.docker.com/r/homeassistant/home-assistant">Home Assistant</a></li>
    <li><a href="https://hub.docker.com/r/portainer/portainer">Portainer</a></li>
    <li><a href="https://hub.docker.com/_/eclipse-mosquitto">Mosquitto</a></li>
    <li><a href="https://hub.docker.com/r/organizrtools/organizr-v2">Organizr</a></li>
    <li><a href="https://hub.docker.com/r/plexinc/pms-docker">Plex</a></li>
    <li><a href="https://hub.docker.com/r/abiosoft/caddy">Caddy</a></li>    
    <li><a href="https://hub.docker.com/r/v2tec/watchtower">Watchtower</a></li> 
    <li><a href="https://hub.docker.com/r/nodered/node-red-docker">Node-RED</a></li>
    <li><a href=https://github.com/Koenkk/zigbee2mqtt">Zigbee2mqtt</a></li></ul>
    </details>

# Front End Screen Shots:
## Settings
<p align="center">
  <img src="https://raw.githubusercontent.com/subjectbit/homeassistant/master/ui/settings_ui.png">
</p>

