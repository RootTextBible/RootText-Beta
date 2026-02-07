# RootText System Requirements
**Last Updated: February 2026**

This document outlines the minimum and recommended system requirements for running the RootText Bible Study application.

---

## Quick Reference

| Component     | Minimum                       | Recommended                    |
|---------------|-------------------------------|--------------------------------|
| OS            | Windows 10 (version 2004+)    | Windows 10 22H2 / Windows 11   |
| Architecture  | x64 only                      | x64                            |
| Processor     | Dual‑core 1.5 GHz             | Quad‑core 2.0 GHz+             |
| RAM           | 4 GB                          | 8 GB+                          |
| Storage       | 15 GB free                    | 20 GB free (SSD)               |
| Display       | 1280 × 720                    | 1920 × 1080+                   |
| Internet      | Required for install          | Required for AI features       |

---

## Detailed Requirements

### Operating System

| Supported? | OS / Version                    | Notes                          |
|-----------|----------------------------------|--------------------------------|
| ✅        | Windows 11                       | Full support                   |
| ✅        | Windows 10 version 2004+         | Build 19041+                   |
| ❌        | Windows 10 earlier than 2004     | Not supported                  |
| ❌        | Windows XP, 7, 8.x               | Not supported                  |
| 🔜        | Windows ARM64                    | Planned                        |
| 🔜        | macOS                            | Planned                        |
| 🔜        | iOS                              | Planned                        |
| 🔜        | Android                          | Planned                        |
| ❌        | Linux                            | Not supported                  |

**Why Windows 10 version 2004+?**
- Required for .NET 9 Desktop Runtime  
- Required for Windows App SDK 1.6  
- Required for WebView2 (Edge-based rendering)

---

### Processor (CPU)

| Requirement | Specification                     |
|------------|------------------------------------|
| Minimum    | 64‑bit dual‑core, 1.5 GHz          |
| Recommended| 64‑bit quad‑core, 2.0 GHz+         |

**Notes**
- ARM64 is not currently supported  
- 32‑bit processors not supported  
- More cores improve database import performance  

---

### Memory (RAM)

| Requirement | Specification | Use Case                   |
|------------|---------------|-----------------------------|
| Minimum    | 4 GB          | Basic Bible reading         |
| Recommended| 8 GB+         | AI features, parallel study |

**Typical memory usage:**
- Application: 200–400 MB  
- Database queries: 500 MB – 1 GB  
- AI/Semantic Kernel: 200–500 MB  
- WebView2 rendering: 100–200 MB  

---

### Storage

| Item                     | Size        |
|--------------------------|-------------|
| Installer download       | ~140 MB     |
| Database download        | ~3 GB       |
| Installed application    | ~200 MB     |
| Extracted database       | 8–10 GB     |
| **Total required**       | **~15 GB**  |

**SSD Recommended**
- Faster installs  
- Faster search performance  
- Much quicker database import  

---

### Display Requirements

| Requirement | Specification        |
|------------|-----------------------|
| Minimum    | 1280 × 720            |
| Recommended| 1920 × 1080 or higher |

Additional notes:
- High‑DPI scaling supported  
- Hebrew/Greek text benefits from higher pixel density  

---

### Internet Connection

| Feature          | Internet Required?  |
|------------------|---------------------|
| Installation     | Yes                 |
| Bible reading    | No                  |
| Search           | No                  |
| AI Study Agent   | Yes                 |
| Updates          | Yes                 |

**Recommended bandwidth**
- 10 Mbps+ for installation  
- Normal broadband for AI features  

---

## Prerequisites (Auto‑Installed)

| Component                          | Size     | Purpose                |
|-----------------------------------|----------|-------------------------|
| Visual C++ Redistributable 2015–2022 | ~25 MB | Runtime libraries      |
| .NET 9 Desktop Runtime            | ~60 MB   | Application framework   |
| Windows App SDK 1.6 Runtime       | ~40 MB   | Modern Windows UI       |

---

## Known Limitations

Not supported:
- Windows on ARM  
- Windows 10 S Mode  
- Windows Server editions (untested)  
- VMs with weak GPU support  

Antivirus considerations:
- May slow installation  
- May flag unsigned installers  
- May slow database import  

---

## Performance Guidelines

### Database Import Time

| Storage Type | Expected Time |
|--------------|---------------|
| NVMe SSD     | 5–8 minutes   |
| SATA SSD     | 8–12 minutes  |
| HDD 7200 RPM | 15–25 minutes |
| HDD 5400 RPM | 25–40 minutes |

### Application Startup Time

| Scenario              | Time        |
|-----------------------|-------------|
| First launch          | 3–5 seconds |
| Subsequent launches   | 1–2 seconds |
| After system reboot   | 2–3 seconds |

---

## Checking Your System

### Check Windows Version
1. Press **Win + R**  
2. Type `winver`  
3. Confirm version **2004 or later**

### Check Free Storage
1. Open **File Explorer**  
2. Select **This PC**

### Check RAM
1. Press **Ctrl + Shift + Esc**  
2. Open **Task Manager → Performance → Memory**

---

## Troubleshooting

### Installer won’t run
- Confirm Windows version  
- Run as Administrator  
- Temporarily disable antivirus  

### Database import is slow
- Use SSD  
- Close other applications  
- Ensure adequate free space  

### Application is slow
- Check available RAM  
- Ensure database is on SSD  
- Install Windows updates  

---

## Future Platform Support

Planned:
- macOS  
- iOS  
- Android  
- Windows ARM64  

Not planned:
- Linux desktop  

---
