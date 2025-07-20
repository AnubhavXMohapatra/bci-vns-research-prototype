# bci-vns-research-prototype
Interactive Python/Jupyter BCI-VNS dashboard fusing simulated autonomic/metabolic markers with live Muse2 alpha-band EEG (via LSL/synthetic fallback). Includes 4×2 plots, clinical insights, and ASCII-safe PDF/CSV/ZIP export. Tracks HRV, vagal tone, stress, glucose, BAT, TNF-α, and energy use.

Real-Time BCI-VNS Simulation Dashboard with Live Muse2 EEG Integration
An interactive Jupyter-based research prototype for spinal cord injury (SCI) neurorehabilitation, combining a multimodal simulation engine, live Muse2 EEG streaming via LSL, advanced visualization, automated clinical insights, and export packaging.

🚀 Key Features
Live Muse2 EEG Toggle “Use Muse2 EEG” to ingest α-band data from a Muse2 headset via Lab Streaming Layer (pylsl). Falls back to a 10 Hz synthetic waveform when no stream is detected.
(your media files (image1.png, image2.png, relaxation.mp3) live in the repo—)
Multimodal Physiological Simulation Models HRV-derived metabolic balance, vagal tone, stress index, blood glucose (80–100 mg/dL), brown adipose tissue (BAT) activation (~12% boost), TNF-α cytokines (< 15 AU), and energy expenditure. Optional circadian, fatigue, nutrition, and medication modulators introduce real-world variability.

Interactive 4×2 Dashboard

Dynamic plots with peak annotations, mean lines, and target zones

Stress heatmap and EEG waveform side-by-side

Full-width scientific reference images with APA citations

Automated Insights & Recommendations

Technical summary referencing PhysioNet MIMIC-IV, OpenNeuro DS000213, PMC Neurorecovery, FDA MAUDE

Personalized nutrition (omega-3s, MCTs, turmeric/flavonoids) and exercise (interval cycling, breathing protocols, cold exposure) plans

One-sentence clinical takeaway

Robust Export & Packaging ASCII-filtered PDF report, detailed CSV session export, and ZIP bundle for reproducibility and collaboration.

🛠️ Installation
Clone this repository

bash
git clone https://github.com/yourusername/bci-vns-dashboard.git
cd bci-vns-dashboard
Create a conda or virtualenv environment

bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
.\venv\Scripts\activate    # Windows
Install dependencies

bash
pip install -r requirements.txt
# requirements.txt includes:
# numpy, pandas, matplotlib, fpdf, ipywidgets, pylsl, jupyterlab
(Optional) Install muselsl for streaming Muse2 data

bash
pip install muselsl
▶️ Usage
Launch JupyterLab / Jupyter Notebook

bash
jupyter lab
Open BCI_VNS_Dashboard.ipynb.

Ensure your Muse2 is streaming via muselsl (e.g. muselsl stream in a separate terminal).

In the notebook’s control panel:

Adjust Duration, Circadian, Fatigue, Food, Medication parameters.

Check Use Muse2 EEG to enable live EEG streaming.

Click Run BCI-VNS to generate real-time plots, insights, and exports.

📂 Repository Structure
├── BCI_VNS_Dashboard.ipynb       # Main interactive notebook
├── requirements.txt             # Python dependencies
├── session_data.csv             # Example CSV export
├── session_summary.pdf          # Example PDF report
├── bci_vns_report.zip           # Example ZIP bundle
├── image1.png / image2.png      # Reference images
└── relaxation.mp3               # Optional audio file
📚 References
Smith et al. (2023). BCI-VNS enhances autonomic recovery in SCI. Journal of Neuroscience

Patel et al. (2022). TNF-α modulation and neuroplasticity post-SCI. Neurorehabilitation and Neural Repair

Lee et al. (2023). Brown adipose tissue activation via cold stimulus. Endocrinology

Jensen et al. (2021). Glucose homeostasis and metabolic stability in SCI. Diabetologia

🤝 Contributing
Contributions, bug reports, feature requests, and pull requests are welcome! Please open an issue or submit a PR.

📧 Contact
Email: your.email@university.edu

Website / Portfolio: yourwebsite.com

LinkedIn: yourprofile

📄 License
This project is released under the MIT License. See LICENSE for details.
