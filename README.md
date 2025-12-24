# 🚀 Antigravity Vibe Template

Ein strukturiertes Start-Template für **Vibe Coding mit AI**.  
Kein Chaos, keine unnötigen Schleifen – sondern ein klarer, organisierter Einstieg mit Regeln, Kontext und Überblick.

Dieses Template richtet sich an Vibecoder, die mit Struktur starten wollen – **mit Plan statt Trial & Error**. 


<div align="center">

**Built for Vibe Coding**


</div>


---

## 🎯 Ziel des Templates

**Organisiert starten. Klar planen. Sauber umsetzen.**

AI kann hervorragend Code generieren –  
aber nur dann wirklich gut, wenn **Guidelines, Regeln und Standards** existieren.

Dieses Template hilft dir dabei:

- von Anfang an **Struktur** zu haben  
- der AI **klaren Kontext** zu geben  
- Änderungen nachvollziehbar zu halten  
- unnötige Tasks und Richtungswechsel zu vermeiden  

> Code ist dank AI schnell geschrieben.  
> Ohne Ziel, Kontext und Planung wird daraus trotzdem kein gutes Projekt.

---

## 📋 Inhaltsverzeichnis

- [Ziel des Templates](#-ziel-des-templates)
- [Warum dieses Template?](#-warum-dieses-template)
- [Erste Schritte](#-erste-schritte)
- [Projektstruktur](#-projektstruktur)
- [Agent-Konfiguration (.agents)](#-agent-konfiguration-agents)
- [DevContainers](#-devcontainers)

---

## ✨ Warum dieses Template?

Vibe Coding bedeutet: **Du + AI im Flow**.  
Aber Flow entsteht nicht durch Zufall, sondern durch Klarheit.

Dieses Template sorgt dafür, dass:

- die AI **nicht raten muss**
- du **den Überblick behältst**
- Regeln früh definiert sind (statt später repariert zu werden)
- Planung vor Code steht

**Ergebnis:**  
Weniger Umwege, weniger Refactoring, mehr Fortschritt.

---

## 🏁 Erste Schritte

1. **Template herunterladen oder klonen**  
   👉 https://github.com/sebastianreinig/vibe_template

2. **Projekt-Kontext definieren**  
   Passe `./.agents/context.md` an  
   > Tipp: Dafür kannst du bereits AI nutzen 😉

3. **Regeln & Struktur akzeptieren**  
   Der Ordner `.agents` ist kein Nice-to-have – er ist zentral.

4. **Loslegen**  
   Mit klarer Richtung, sauberem Setup und Fokus auf das Wesentliche.

---

## 📁 Projektstruktur

```
project-root/
├── .agents/
│   ├── context.md
│   ├── memory.md
│   ├── rules/
│   └── workflows/
├── .devcontainer/
├── changelog.md
├── sbom.md
└── README.md
```

---
## 🤖 Agent-Konfiguration (./.agents/)

Dieser Ordner ist dein wichtigstes Tool. Er verhindert, dass Antigravity Müll produziert.

context.md: Hier sagst du der KI, was die Architektur ist. Kein Raten, nur Wissen.
memory.md: Antigravity merkt sich hier deine Vorlieben. Einmal eingestellt, immer gewusst.
rules/ & workflows/: Standardisiere deine Arbeit, damit du dich nicht mit Kleinkram aufhalten musst.


## 🐳 DevContainers
DevContainers sind nützlich, aber absolut nicht notwendig.

Wenn du ein schnelles Solo-Projekt startest, lass sie einfach weg. Sie sind nur da, falls du eine isolierte Umgebung brauchst oder später doch jemanden zum Vibe Coding einlädst.