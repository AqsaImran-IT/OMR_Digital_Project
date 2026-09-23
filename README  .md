# 📝 Digital OMR Solution

A **PyQt6-based desktop application** for managing an OMR (Optical Mark Recognition) sheet batch-processing workflow — from secure login, to folder selection, to batch "processing," result review, and CSV export — all in one clean dashboard interface.

> ⚠️ **Note:** This is currently a **UI/workflow prototype**. The batch processing simulates results (completed / blank / flagged / not-processed) for demo purposes. The actual OMR bubble-detection / image-recognition logic is not yet implemented — the results table and CSV export are generated using placeholder logic.

---

## ✨ Features

- 🔐 **Login screen** with username/password authentication
- 📁 **Input & Output folder selection** for sheet images and exported results
- 📊 **Live dashboard** with metric cards — Detected, Ready, Pending, Completed, Idle/Blank, Quality Flags, Not Processed, Exports
- ⏳ **Batch processing simulation** with animated progress bar
- 📋 **Results table** showing Sheet Name, Roll No, Score, Quality Flag, and Status per sheet
- 🧾 **CSV export** of batch results to the output folder
- 🗒️ **Processing log** tab for real-time activity tracking
- 🖼️ Sheet preview area with zoom and review-overlay controls (UI only)

---

## 🛠️ Tech Stack

- **Language:** Python 3.11
- **GUI Framework:** PyQt6
- **Data Export:** CSV (via Python's built-in `csv` module)

---

## 📂 Project Structure

```
OMR_Digital_Project/
│
├── Source/                    # Sample OMR sheet images used for testing
├── Output/
│   └── OMR_Results_Export.csv # Generated results after processing
├── main.py                    # Application entry point (all UI + logic)
├── .gitignore
├── LICENSE
└── README.md
```

---

## ⚙️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/AqsaImran-IT/OMR_Digital_Project.git
   cd OMR_Digital_Project
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv .venv
   .venv\Scripts\activate      # Windows
   source .venv/bin/activate   # macOS/Linux
   ```

3. **Install dependencies**
   ```bash
   pip install PyQt6
   ```

4. **Run the application**
   ```bash
   python main.py
   ```

---

## 🚀 Usage

1. Launch the app — you'll land on the **login screen**
2. Sign in with the demo credentials:
   - **Username:** `test`
   - **Password:** `Test123`
3. On the dashboard:
   - Select an **Input Directory** containing `.jpg` / `.jpeg` / `.png` sheet images
   - Select an **Output Directory** for results
   - Click **Check Batch Status** to see how many sheets were detected
   - Click **Start Processing** to run the batch (progress bar simulates processing)
4. View results in the **Results** tab, or check the **Processing Log** tab for activity
5. Click **Open Output Folder** to access the exported `OMR_Results_Export.csv`

---

## 🗺️ Roadmap

- [ ] Implement actual OMR bubble-detection using image processing (e.g. OpenCV)
- [ ] Add real answer-key based scoring
- [ ] Replace hardcoded login credentials with secure authentication
- [ ] Add sheet preview rendering in the Dashboard tab

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👩‍💻 Author

**Aqsa Imran**
GitHub: [@AqsaImran-IT](https://github.com/AqsaImran-IT)
