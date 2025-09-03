# Fourier Analysis – Signals and Systems (Parcial 2)

This repository contains the implementation of **Parcial 2** for the course *Signals and Systems* at the **National University of Colombia – Manizales Campus**.  
The project is developed in **Python** using **Streamlit** for the interactive interface and **Ngrok** for public deployment.  

---

## Contents

The Streamlit app includes four main sections related to Fourier analysis:

1. **Fourier Spectrum Expression**  
   - Derivation of Fourier coefficients in trigonometric and exponential form.  
   - Visualization of the signal and its components.  

2. **Simulation and Fourier Spectrum**  
   - Numerical simulation of Fourier series.  
   - Visualization of basis functions, coefficients, and signal reconstruction.  
   - Error estimation and Bode diagram plotting.  

3. **Amplitude Modulation (AM) with Audio**  
   - Audio download from YouTube using `yt-dlp`.  
   - Conversion and modulation in AM with adjustable modulation index.  
   - Time-domain and frequency-domain analysis of message, carrier, and modulated signals.  

4. **Total Harmonic Distortion (THD) and Power Factor**  
   - Simulation of rectifiers with resistive and RC loads.  
   - Computation of THD and power factor.  
   - Fourier spectrum analysis of current signals.  

---

## Running the Project

### 1. Install Dependencies (Colab or Local)
```bash
pip install streamlit pyngrok yt-dlp soundfile pydub matplotlib numpy scipy
sudo apt-get install ffmpeg
```

### 2. Run Streamlit
```bash
streamlit run app.py --server.port 8501
```

### 3. Expose with Ngrok (Optional)
```python
from pyngrok import ngrok
ngrok.set_auth_token("YOUR_TOKEN")
public_url = ngrok.connect(8501)
print(public_url)
```

This will provide a public URL to access the Streamlit app.

---

## Repository Structure
```
app.py           # Main Streamlit application
requirements.txt # Project dependencies
README.md        # Project documentation
```

---

## Course Information
- **Course:** Signals and Systems – Fourier Analysis  
- **Institution:** Universidad Nacional de Colombia, Sede Manizales  
- **Semester:** 2024-1  
- **Authors:**  
  - Andrés Fernando Sospanta López  
  - Juan Camilo Perdomo Soto  

---

## Requirements
- Python 3.10+  
- Streamlit  
- Pyngrok  
- yt-dlp  
- Pydub  
- Soundfile  
- Numpy, Scipy, Matplotlib  

---

## License
This repository is intended for academic purposes only as part of coursework at the National University of Colombia.  
