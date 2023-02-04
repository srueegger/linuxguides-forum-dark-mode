# LinuxGuides Forum Dark Theme
Ein CSS-Theme für das <a href="https://github.com/openstyles/stylus" target="_blank">Stylus Addon</a>.
<br><br>
Wenn der Systemweite Dunkelmodus (Dark Mod) im Betriebssystem aktiviert ist, wird das <a href="https://forum.linuxguides.de/" target="_blank">LinuxGuides Forum</a> dank dieser CSS Datei ebenfalls in einem dunklen Theme dargestellt.
<br>

## Wie funktioniert dieses Addon
<ol>
  <li>Als ersten Schritt muss man sich das Stylus Addon für seinen Browser herunterladen. <strong>Achtung</strong> unter Linux funktioniert dieses Theme nur im Firefox Browser.
    <ul>
      <li><a href="https://addons.mozilla.org/de/firefox/addon/styl-us/" target="_blank">Download für Mozilla Firefox</a></li>
      <li><a href="https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne" target="_blank">Download für Google Chrome</a></li>
      <li><a href="https://addons.opera.com/de/extensions/details/stylus/" target="_blank">Download für Opera</a></li>
    </ul>
  </li>
  <li>
    Das Theme installieren: <a target="_blank" href="https://userstyles.world/style/8460/linuxguides-forum-dark-theme">https://userstyles.world/style/8460/linuxguides-forum-dark-theme</a>
  </li>
  <li>
    Den Dark Mode im Betriebssystem aktivieren
  </li>
</ol>

## Theme selber kompilieren
Wen du das Theme selber kompilieren möchtest. Musst du Node.js in der Version 18.x LTS installiert haben.

Am einfachsten installierst du Node.js als Snap

```bash
sudo snap install node --classic --channel=18
```

Danach muss man SASS installieren

```bash
sudo npm install -g sass
```

Nach dem klonen des Repository, kann man innerhalb vom Repository zwei Befehle ausführen.

```bash
npm run sass-dev
```

oder

```bash
npm run sass-prod
```

Der Befehl "sass-dev" - lässt einen Task-Watcher laufen. Der bei jeder Änderung einer SCSS Datei, automatisch die main.css neu kompiliert.

Wen man mit den Änderungen zufrieden ist, kann man mit "sass-prod" die finale CSS-Datei erstellen. "sass-prod" kompiliert ebenfalls die main.css, diesmal aber minimiert.

## License
[The GPL License (GPL V2)](https://github.com/srueegger/linuxguides-forum-dark-mode/blob/main/LICENSE)
<br>