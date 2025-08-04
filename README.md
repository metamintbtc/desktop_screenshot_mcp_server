# Screenshot MCP Server 📸

Ein hochmoderner **Model Context Protocol (MCP) Server** für Windows-Screenshots, entwickelt mit **.NET 10**. Dieser Server simuliert die **Print Screen** Funktionalität und ermöglicht es AI-Assistenten, Screenshots zu erstellen.

## ✨ Features

- 🖥️ **Multi-Monitor Support**: Screenshots aller Bildschirme gleichzeitig
- 🎯 **Primärer Bildschirm**: Screenshots nur des Hauptbildschirms  
- 📊 **Bildschirm-Info**: Detaillierte Informationen über alle Displays
- 🚀 **Print Screen Simulation**: Genau wie die Windows Print Screen Taste
- 💾 **Workspace Integration**: Screenshots werden im aktuellen Workspace gespeichert
- ⚡ **State-of-the-Art**: Neueste .NET 10 Technologie

## 🛠️ Installation

### Über NPM (Empfohlen)
```bash
npm install -g screenshot-mcp-server
```

### Manuell via Git
```bash
git clone https://github.com/yourusername/screenshot-mcp-server.git
cd screenshot-mcp-server
dotnet build
```

## 🚀 Verwendung

### In VS Code mit GitHub Copilot

1. **MCP Server konfigurieren** in VS Code Settings:
```json
{
  "github.copilot.chat.mcp.servers": {
    "screenshot-mcp-server": {
      "command": "dotnet",
      "args": ["run", "--project", "ScreenshotMcpServer.csproj"],
      "description": "Windows Screenshot Server"
    }
  }
}
```

2. **Server starten**:
   - Öffnen Sie die Command Palette (`F1`)
   - Suchen Sie nach "MCP: List Servers"
   - Wählen Sie "screenshot-mcp-server"

### Verfügbare Tools

#### 📸 `TakeScreenshot`
Macht einen Screenshot aller Bildschirme (simuliert Print Screen)
```
Erfasst alle Monitore gleichzeitig
Speichert als PNG im aktuellen Workspace
Dateiname: screenshot_2025-08-04_18-59-30.png
```

#### 🎯 `TakePrimaryScreenshot`  
Macht einen Screenshot nur vom primären Bildschirm
```
Erfasst nur den Hauptmonitor
Ideal für fokussierte Screenshots
Dateiname: primary_screenshot_2025-08-04_18-59-30.png
```

#### 📊 `GetScreenInfo`
Zeigt detaillierte Informationen über alle Bildschirme
```
- Anzahl der Monitore
- Auflösungen und Positionen  
- Virtueller Desktop Größe
```

#### ⌨️ `SimulatePrintScreen`
Emuliert exakt den Windows Print Screen Tastendruck

## 💻 Systemanforderungen

- **OS**: Windows 10/11 (x64)
- **.NET**: .NET 10.0 oder höher
- **RAM**: Mindestens 512 MB
- **Storage**: 50 MB freier Speicherplatz

## 🔧 Entwicklung

### Build
```bash
dotnet build ScreenshotMcpServer.csproj
```

### Run  
```bash
dotnet run --project ScreenshotMcpServer.csproj
```

### Publish
```bash
dotnet publish -c Release -o ./dist
```

## 📁 Projekt Struktur

```
screenshot-mcp-server/
├── Program.cs              # Haupteinstiegspunkt
├── ScreenshotTool.cs      # Screenshot-Funktionalität
├── ScreenshotMcpServer.csproj # .NET Projekt
├── package.json           # NPM Konfiguration
├── README.md             # Diese Datei
└── bin/                  # Compilierte Binaries
```

## 🤝 Contributing

1. Fork das Repository
2. Erstelle einen Feature Branch (`git checkout -b feature/amazing-feature`)
3. Commit deine Änderungen (`git commit -m 'Add amazing feature'`)
4. Push zum Branch (`git push origin feature/amazing-feature`)  
5. Öffne einen Pull Request

## 📄 Lizenz

Dieses Projekt ist unter der MIT Lizenz veröffentlicht. Siehe [LICENSE](LICENSE) für Details.

## 🔗 Links

- [Model Context Protocol](https://modelcontextprotocol.io/)
- [.NET 10 Documentation](https://docs.microsoft.com/en-us/dotnet/)
- [VS Code GitHub Copilot](https://code.visualstudio.com/docs/copilot/)

## 🆘 Support

Bei Problemen oder Fragen:
- 📧 Email: info@screenshot-mcp.dev
- 🐛 Issues: [GitHub Issues](https://github.com/yourusername/screenshot-mcp-server/issues)
- 💬 Discussions: [GitHub Discussions](https://github.com/yourusername/screenshot-mcp-server/discussions)

---

**Made with ❤️ for the AI Community**
