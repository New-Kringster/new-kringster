# Hello. I'm Braven.

Most projects need hardware, software and design, and I like doing all three myself.

I'm a third-year Electronic and Computer Engineering student at Nanyang Polytechnic in Singapore. I started by taking apart a broken radio to see how it worked, and now I design circuit boards, write firmware, build web apps and run the homelab they live on. Every project below has a full write-up on my website, [chiambucket.com](https://www.chiambucket.com).

<br>

## Flagship project

### OCR Reader

<a href="https://www.chiambucket.com/waterslop"><img src="https://www.chiambucket.com/images/ocr-reader-flagship.webp" alt="The OCR Reader board, an ESP32-S3 with a camera, next to the DrumNet model reading the digits of a water meter" width="100%"></a>

A battery-powered camera that reads a water meter, entirely on the chip. I built it end to end, from a four-layer board around an ESP32-S3 and an OV2640 camera to a case that snaps shut with side clips and no screws. DrumNet, a 693K-parameter network, finds the drums on the meter, reads each digit three times and votes on it in about two seconds, so only the number goes out over LoRaWAN.

**693K** parameter model · **~2 s** per reading · **4-layer** custom PCB · **LoRaWAN** low-power link

[Read the article](https://www.chiambucket.com/waterslop) · [Open the report](https://www.chiambucket.com/downloadable/ocr-reader-report.pdf)

<br>

## Highlights

### Project June

<a href="https://www.chiambucket.com/project-june"><img src="https://www.chiambucket.com/images/home/june-banner.webp" alt="The Project June rover kicking up dirt, with an Xbox controller and a laptop showing three live camera feeds" width="100%"></a>

A 5G rover I can drive anywhere there is signal. Three phones on the rover act as its 5G hotspots and cameras, and each one streams its view to my web console over WebRTC while an ESP32-S3 sends GPS, temperature, humidity and light readings back over MQTT about ten times a second. I drive it with an Xbox controller, and the commands and video travel through my own MQTT and TURN servers with about a second of delay from over 8 km away. It took three weeks to go from the first concept to the first drive.

**3** live video streams · **5G** cellular link · **8+** onboard sensors · **3 weeks** concept to drive

[Read the article](https://www.chiambucket.com/project-june) · [Watch the build](https://youtu.be/MnkJsx-nwoE) · [Code](https://github.com/New-Kringster/ProjectJune)

### Pip

<a href="https://www.chiambucket.com/pip"><img src="https://www.chiambucket.com/images/pip-pf-context.webp" alt="Pip, a small teal character waving from the screen of an M5Stack Tab5" width="100%"></a>

A desk pet with an AI agent for a brain, which I built during my internship at M5Stack. Pip lives on an M5Stack Tab5, while its brain is the DeepSeek Harness on my server, so it can drive a browser, build its own apps and keep an eye on my other agents. When I ask it to show me something, it takes a screenshot of the page, finds the part in the picture and draws a circle, an arrow and a note over it. The apps it writes are either Lua scripts that run on the tablet or web apps it serves from my server, and it keeps them in a drawer for later.

**106 s** to build a timer app · **Lua** native applets · **Docker** web applets · **1** desktop for every chat

[Read the article](https://www.chiambucket.com/pip)

### BeadReader

<a href="https://www.chiambucket.com/beadreader"><img src="https://www.chiambucket.com/images/beadreader-pf-context.webp" alt="Three phones showing the BeadReader sign-in page, a chapter of a book and the library" width="100%"></a>

A private book reader for a few friends. I publish books in Markdown or as webtoons, my friends sign in with one access code, and anyone on the same book can see the others reading live. Tapping your own row in the reading list opens the chapter at the line you stopped on, and you can send a friend a wave or a short note that fades from their screen in seconds and is never saved. It is built with Next.js and Supabase, and anyone can deploy their own copy in one click.

**Live** read-together presence · **SQL-enforced** content gate · **Offline** reading · **1 click** to deploy your own

[Read the article](https://www.chiambucket.com/beadreader) · [Code](https://github.com/New-Kringster/BeadReader)

<br>

## More projects

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://www.chiambucket.com/lumen"><img src="https://www.chiambucket.com/images/lumen-pf-context.webp" alt="The LUMEN smart home assistant, an ESP32 board with the OpenAI Whisper and DeepSeek logos" width="100%"></a>
      <h3>LUMEN</h3>
      <p>A voice-controlled room on an ESP32, where Whisper and DeepSeek turn what I say into one JSON command that is sent over MQTT.</p>
      <p><sub>School project</sub><br><a href="https://www.chiambucket.com/lumen">Read the article</a></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://www.chiambucket.com/pantry"><img src="https://www.chiambucket.com/images/pantry-pf-context.webp" alt="The Pantry Expiry Tracker, an M5Stack CoreS3 SE stacked on a barcode scanner module" width="100%"></a>
      <h3>Pantry Expiry Tracker</h3>
      <p>An expiry tracker for the fridge door, where you scan a barcode, pick when it expires and the screen shows what to eat first.</p>
      <p><sub>Internship project, M5Stack</sub><br><a href="https://www.chiambucket.com/pantry">Read the article</a> · <a href="https://github.com/New-Kringster/Pantry_tracker_code">Code</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://www.chiambucket.com/scroll-ruler"><img src="https://www.chiambucket.com/images/scroll-ruler-pf-context.webp" alt="The Scroll Ruler, an M5Stack AtomS3R on top of a Unit Scroll wheel" width="100%"></a>
      <h3>Scroll Ruler</h3>
      <p>A digital ruler made from an AtomS3R and a Unit Scroll, which measures whatever you roll its wheel along.</p>
      <p><sub>Internship project, M5Stack</sub><br><a href="https://www.chiambucket.com/scroll-ruler">Read the article</a> · <a href="https://github.com/New-Kringster/AtomS3R_ScrollWheelRuler">Code</a></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://www.chiambucket.com/brolocator"><img src="https://www.chiambucket.com/images/borlocator-pf-context.webp" alt="Two ESP32 LoRa handhelds standing side by side" width="100%"></a>
      <h3>LoRa Messenger</h3>
      <p>Two ESP32 handhelds on my first PCB, which send text over LoRa and rough two-way voice over ESP-NOW.</p>
      <p><sub>Personal project</sub><br><a href="https://www.chiambucket.com/brolocator">Read the article</a> · <a href="https://github.com/New-Kringster/Bro_Locator">Code</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://www.chiambucket.com/csdp"><img src="https://www.chiambucket.com/images/Ema-pf-context.webp" alt="A small black EMA Labs smart home node with a cable" width="100%"></a>
      <h3>EMA Smart Home</h3>
      <p>A team smart home, graded A, where four BeagleBone Black nodes report to a Socket.IO server with a live 3D dashboard.</p>
      <p><sub>School project</sub><br><a href="https://www.chiambucket.com/csdp">Read the article</a> · <a href="https://github.com/New-Kringster/EMA-Smart-home-System">Code</a></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://www.chiambucket.com/elecf"><img src="https://www.chiambucket.com/images/elef2-pf-context.webp" alt="The ELEC-F freezer alarm concept" width="100%"></a>
      <h3>ELEC-F Concept</h3>
      <p>A walk-in freezer alarm on M5Stack that starts counting down when someone is shut inside.</p>
      <p><sub>School project</sub><br><a href="https://www.chiambucket.com/elecf">Read the article</a> · <a href="https://github.com/New-Kringster/ELEC-F-Safe-Fridge-Concept">Code</a></p>
    </td>
  </tr>
</table>

I have a few more on the go, and their write-ups are coming soon:

- **Series One Light**, an ultralight gaming mouse shell based on the ZeroMouse, which I am aiming to bring down to about 20 g.
- **Copy Board**, a KiCad recreation of my school's dev board, which I made because I couldn't bring the original home.
- **Minecraft Live Map**, a Paper server in Docker on my homelab with a live Dynmap of the world.
- **[Pandus Dispenser](https://www.chiambucket.com/pandus)**, my first school project, which is a six-part 3D-printed syrup dispenser run by an Arduino Uno.
