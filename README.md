# About the setup
<details>
<summary>
  <b>Compute & Detection</b></summary>
  <ul>
  <li><a href="https://www.intel.com/content/www/us/en/products/boards-kits/nuc/kits/nuc7i5bnh.html">Intel NUC</a></li>
  <li><a href="https://phoscon.de/en/conbee2">Conbee II</a></li>
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
  <p>I like using Xiaomi sensors as they're cheap, reliable, and portable. This is especially relevant to my use case as I bought the majority of the sensors used in my setup as a renter. I've since graduated to home ownership and have mounted the sensors in key areas to detect motion, climate, and door/window settings. All the Xiaomi sensors and switches are controlled via the deCONZ container with a Conbee 2 coordinator. I originally used the zigbee2mqtt container with the CC2531 but experienced constant stability issues. Ever since getting past the initial setup with deCONZ, it's been rock solid.</p>
  <ul>
  <li><a href="https://www.aliexpress.com/item/New-Original-Xiaomi-Mijia-Human-Body-Sensor-Infrared-Smart-Home-Detector-Motion-Sensor-Safe-Moistureproof-15ms/32858852215.html?spm=2114.search0104.3.19.111f316b2zfoj2&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10902_10059_10884_10887_321_322_10103,searchweb201603_57,ppcSwitch_0&algo_expid=cfc297f2-d6a6-4952-a632-a63ac3f66fdd-2&algo_pvid=cfc297f2-d6a6-4952-a632-a63ac3f66fdd">Xiaomi Mijia Human Body Sensor</a></li>
  <li><a href="https://www.aliexpress.com/item/2019-Xiaomi-Mi-Smart-Temperature-and-Humidity-Sensor-Mini-Intelligent-Sensor-Put-the-baby-Home-office/32986664949.html?spm=2114.search0104.3.32.17e2205013KSAz&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10902_10059_10884_10887_321_322_10103,searchweb201603_57,ppcSwitch_0&algo_expid=246f6dd6-c260-492f-82da-5b9358ca0864-7&algo_pvid=246f6dd6-c260-492f-82da-5b9358ca0864">Xiaomi Mi Smart Temperature & Humidty</a></li>
  <li><a href="https://www.aliexpress.com/item/Xiaomi-Aqara-Wireless-Flood-Water-Immersing-Sensor-IP67-Waterproof-App-Remote-Cantrol-Remote-Mijia-Smart-Home/32921707280.html?spm=2114.search0104.3.55.69e2fec1u0Ht7A&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10902_10059_10884_10887_321_322_10103,searchweb201603_57,ppcSwitch_0&algo_expid=9c9b4499-285b-4f4c-9fee-6efad92b8e55-7&algo_pvid=9c9b4499-285b-4f4c-9fee-6efad92b8e55">Xiaomi Aqara Water Sensor</a></li>
  <li><a href="https://www.aliexpress.com/item/HOT-Original-Xiaomi-Door-Window-Sensor-Pocket-Size-Xiaomi-Smart-Home-Kits-Alarm-System-Work-with/32965692266.html?spm=2114.search0104.3.17.17c12c44nGAg85&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10902_10059_10884_10887_321_322_10103,searchweb201603_57,ppcSwitch_0&algo_expid=bfe0ecfe-0bb3-4e45-a9b7-678244bb4d78-2&algo_pvid=bfe0ecfe-0bb3-4e45-a9b7-678244bb4d78">Xiaomi Door/Window Sensor</a></li>
  </ul>
</details>
<details>
<summary>
  <b>Lighting</b></summary>
  <p>After experimenting with wi-fi bulbs, I decided to leverage Zigbee for all lighting. In my current setup, I have 50+ bulbs in action with the majority coming from the Philips Hues lineup. I've never used the official hub as I prefer to use a more genericized hub to reduce vendor dependencies. To that end, I've had great success using the deCONZ software with the Conbee II coordinator. Setting up lights is simple and performance is rock solid.</p>
  <ul>
  <li><a href="https://www2.meethue.com/en-us">Philips Hues</a></li>
  <li><a href="https://www.ikea.com/us/en/catalog/categories/departments/living_room/36812/">TRÅDFRI</a></li>
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
    <li><a href="https://github.com/pyouroboros/ouroboros">Ouroboros</a></li> 
    <li><a href="https://hub.docker.com/r/nodered/node-red-docker">Node-RED</a></li>
    <li><a href=https://github.com/marthoc/docker-deconz">deCONZ</a></li></ul>
    </details>

# UI Screenshots

## Overview
<p>The overview page gives a quick snapshot of activity in the house. Some elements such as media players and any open doors or windows are dynamic and only appear while in certain states (e.g. an open window). I've shifted my approach to the UI in general by trying to use it less in favor of building intuitive contexts and automations. </p>
<p align="center">
  <img src="https://raw.githubusercontent.com/subjectbit/homeassistant/master/ui/overview_ui.png">
</p>

## Basement
<p>Rather than taking a room by room view approach, I've pared down each view to represent the floor (basement, first, second). </p>
<p align="center">
  <img src="https://raw.githubusercontent.com/subjectbit/homeassistant/master/ui/basement.png">
</p>

## First Floor

<p>Each column represents different spaces. My home has a very open first floor layout so blending the different lighting and motion contexts is important.</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/subjectbit/homeassistant/master/ui/first_floor.png">
</p>

## Second Floor

<p>I've tried to use a consistent hierarchy in each view by displaying motion and lights, then media players, then any additional sensors such as climate or window/door status.</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/subjectbit/homeassistant/master/ui/second_floor.png">
</p>


## Settings

<p>For now, I've added some simple views and controls to manage each container and automation status. Eventually, I'll migrate most of this to a Grafana dashboard to help understand long term trends of consumption and use.</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/subjectbit/homeassistant/master/ui/settings_ui.png">
</p>

