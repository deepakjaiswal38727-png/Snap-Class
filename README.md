# Snap-Class: Multimodal AI Attendance System 🚀

Snap-Class is an automated, high-security attendance tracking ecosystem that replaces traditional roll calls. By leveraging a multimodal biometric pipeline—combining **Deep Learning Face Recognition** and **Neural Voice Verification**—it ensures spoof-proof, frictionless identity verification in real time.

---

## ⚡ System Architecture & Core Pipelines

| Pipeline / Layer | Technology | Operational Function |
| :--- | :--- | :--- |
| **Frontend UI** | Streamlit | Responsive web-app container, role-based screen routing. |
| **Face Engine** | `dlib`, `face_recognition_models` | 68-point facial landmark mapping & deep vector encoding. |
| **Voice Engine** | `resemblyzer`, `librosa` | Raw audio processing & speaker embedding extraction. |
| **Backend & DB** | Supabase (PostgreSQL Client) | Real-time secure logging, student enrollment data management. |
| **Security** | `bcrypt` | Cryptographic password hashing for user access controls. |
| **Utilities** | `segno`, `pillow` | Dynamic instant QR code generation for classroom session sharing. |

---

## 📂 Repository Structure

```text
├── ai-attendance-project-app-main/
│   ├── app.py                     # Main application entry point (Streamlit)
│   ├── requirements.txt           # Python project dependencies
│   └── src/
│       ├── components/            # UI Modals (enrollment, voice capturing, logs)
│       ├── database/              # Cloud backend connections & schema configs
│       ├── pipelines/             # Core AI processors (face_pipeline.py & voice_pipeline.py)
│       └── screens/               # Execution portals (home, student, teacher)
