# penansible
Ansible Setup QEMU-VM mit x-resize und Burp Suite Professional

Dieses Ansible-Projekt richtet eine Kali Linux VM mit automatischem Display-Resize-Skript (x-resize) und Burp Suite Professional ein.

## Voraussetzungen

- Ansible (neueste Version)
- SSH-Zugang zu der VM, auf der das Setup ausgeführt werden soll (Kali Linux)
- Burp Suite Professional Lizenzschlüssel

## Projektstruktur

Das Playbook lädt und installiert automatisch:

- Das `x-resize` Skript und eine passende udev-Regel, um die Anzeige bei Fenstergrößenänderung automatisch anzupassen.
- Burp Suite Professional in der neuesten Version mit Installation des License Keys (Lizenzschlüssel wird interaktiv abgefragt).

## Nutzung

1. Repository klonen:

```commandline
git clone <dein-repo-url>
cd ansible-kali-burp
```


2. Playbook ausführen:

```commandline
ansible-playbook -i <inventar-datei> playbook.yml
```


3. Während der Ausführung wirst du aufgefordert, den Burp Suite Lizenzschlüssel einzugeben.

## Hinweise

- Das automatische Eintragen des Lizenzschlüssels in Burp Suite kann je nach Version manuelle Schritte oder eine separate Lizenzdatei erfordern.
- Das Playbook richtet das notwendige Paket- und Dienst-Setup für x-resize und QEMU Integration ein.
- Die URL für Burp Suite wird auf die offizielle Download-Seite verwiesen, ggf. muss ein Login erfolgen.

---


