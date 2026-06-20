````markdown
# IVR Visual Flow Builder - Enterprise Node Editor

> **🔒 Proprietary Software Disclaimer**
> This repository is maintained strictly as an architectural showcase. The source code is proprietary, built for a telecommunications/B2B environment. No closed-source logic or internal infrastructure data is published here.

The IVR Visual Flow Builder is an advanced, highly interactive node-based editor designed to map out, manage, and deploy complex Interactive Voice Response (IVR) call flows for enterprise call centers and Asterisk-based PBX systems. 

## 📸 Platform Previews

<!-- Add your screenshots to the repository and update the filenames below -->
### 🎛️ Visual Canvas & Drag-and-Drop Interface
![Flow Canvas Preview](./canvas.png)

### ⚙️ Node Configuration & Context Menus
![Node Configuration](./node-config.png)

## 🎯 Project Overview & Business Value
Designing call routing logic manually via code or basic dropdowns is highly prone to errors and inaccessible to non-technical managers. This platform solves that by introducing a visual paradigm:
* **No-Code Call Routing:** Allows operations managers to visually drag, drop, and connect IVR nodes to build customer journeys.
* **Telecom Integration:** Directly translates visual flowcharts into executable telecom commands (e.g., Asterisk Dialplan).
* **Reduced Time-to-Market:** Cuts down the time required to deploy new call center campaigns from days to minutes.

## 🏛 Technical Architecture

Building a node-based interface requires intricate state management, canvas calculation, and modular component design.

* **Core Framework:** React.js (with custom hooks for canvas state manipulation).
* **Build System:** Webpack & Babel optimized for heavy client-side processing.
* **UI/UX Components:** Custom Menubars, Context Menus, and dynamic Sidebars for node property editing.

## 🚀 Key System Features & Node Types

The engine supports a wide array of specialized telecommunication nodes, including but not limited to:
* **Interaction Nodes:** `InputNode`, `InputVoiceNode`, `SwitchNode` (for complex logic branching).
* **Media Nodes:** `PlaybackNode`, `PlayToneNode`, `RecordNode`.
* **Telephony Actions:** `DialNode`, `HangUpNode`, `SendFaxNode`, `AsteriskCmdNode` (direct integration with Asterisk PBX).
* **Logic & Variables:** `IfNode`, `SetNode`, `GoToNode`, `RpcNode` (for external API triggers).

## 📄 Deployment Note
The application is bundled via Webpack into optimized static assets (`bundle.js`) for seamless deployment across modern web servers.
