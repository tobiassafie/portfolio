# Tobias Safie - Portfolio
[toby.safie@gmail.com](mailto:toby.safie@gmail.com) | [tks57@drexel.edu](mailto:tks57@drexel.edu) | [linkedin.com/in/tsafie](linkedin.com/in/tsafie)
---

I am a Physics, Economics, and Mathematics triple major at Drexel University in Philadelphia, PA and this is a curated selection of my favorite work across **physics**, **machine learning**, and **quantitative finance**.
<br><br>
Each repository is linked in the **title** of each listed project.

---

## Featured Projects

### [**NASA Fermi GRB Clustering**](https://github.com/tahumada/GBM-ML)
Developed ML pipelines for the **unsupervised clustering** of over 750k high-noise **gamma-ray bursts (GRBs)** to identify outlier astrophysical events detected by the Fermi Telescope. This is a sub-project under a wider multi-stage project created by my mentor, Dr. Niharika Sravan, to create an ML pipeline for NASA's radio team.
<br>
_This project was tackled under the mentorship of and collaboration with Dr. Niharika Sravan and Dr. Tomas Ahumada_
<br><br>
**Tools:** Python, PyTorch, Scikit-Learn, Pandas, DataWrangler, GoogleCloud, UMAP, t-SNE, PCA
<br>
**Highlights:**
- Built high-dimensional autoencoder pipelines to extract latent features from raw GRB time series
- Utilized academic and industry standard architectures including: Transformer, CNN, LSTM, TS2-Vec
- Optimized handling of >750k bursts × 14 detectors × ~1k timesteps (≈10¹⁰ total data points)
- Applied clustering and dimensionality reduction (t-SNE, PCA) to identify hidden temporal–spectral patterns
<br>
<div align = "center">
<table>
  <tr>
    <td align="center">
      <img src="assets/tsne_projection.png" width="400px" alt="t-SNE Projection"><br>
      <em>t-SNE projection of latent GRB features</em>
    </td>
    <td align="center">
      <img src="assets/pca_projection.png" width="400px" alt="PCA Projection"><br>
      <em>PCA projection of latent GRB features</em>
    </td>
  </tr>
</table>
</div>

<br>

### [**Physics-Informed Neural Networks for Options Pricing**](https://github.com/tobiassafie/STAR)
Developed and benchmarked Physics-Informed Neural Networks (PINNs) to approximate nonlinear partial differential equations (PDEs) across domains in physics and ultimately derivative pricing models. 
<br>
_Conducted as part of Drexel’s Students Tackling Advanced Research (STAR) Scholars program during Summer '25._
<br>
**Tools:** Python, PyTorch, Pandas, NumPy, Kaggle
<br>
**Highlights:**
- Built PyTorch-based PINN framework to approximate nonlinear PDEs in physics and quantitative finance  
- Implemented the Heston stochastic volatility and Black–Scholes models using physics-informed constraints  
- Benchmarked against RK4 solvers and finite-difference methods for stability and convergence analysis  
- Produced high-resolution solution surfaces, residual heatmaps, and model ablation studies  
- Designed architecture modularity for extension to inverse problems and multi-physics coupling
<br>
<div align = "center">
<table>
  <tr>
    <td align="center">
      <img src="assets/blackscholes_pinn_solution.png" width="400px"><br>
      <em>Black-Scholes PDE solution surface predicted by PINN</em>
    </td>
    <td align="center">
      <img src="assets/1D_diffusion.gif" width="400px"><br>
      <em>PINN-predicted solution of the 1D diffusion equation over time (test case)</em>
    </td>
  </tr>
</table>
</div>
<br>

### [**Fast Radio Burst FPGA Classifier**](./frb/simple_model_accuracy.ipynb) - _Work in Progess_
Designing a real-time inference pipeline to detect and classify Fast Radio Bursts (FRBs) from live telescope data. The project integrates machine-learning models with low-level hardware acceleration for efficient and low-latency on-device signal processing.
<br>
_Another project developed under Dr. Niharika Sravan that has seen many collaborators and contributors._
<br>
**Tools:** Python, TensorFlow, Verilog, C++, Scikit-Learn, hls4ml, FPGA
<br>
**Highlights:**
- Building an end-to-end pipeline for FRB detection and classification using CNN architectures
- Converting trained Sk-Learn models to low-level representations for deployment on an FPGA
- Implementing real-time signal ingestion and preprocessing for telescope data streams
- Targeting efficient inference under strict parameter and memory constraints (<100k parameters)

<div align = "center">
<table>
  <tr>
    <td align="center">
      <img src="assets/frb_roc_curve.png" width="400px" alt="ROC Curve – FRB vs RFI"><br>
      <em>Historic ROC curve for FRB classifier showing strong discrimination (AUC = 0.967)</em>
    </td>
    <td align="center">
      <img src="assets/fpga.png" width="400px" alt="FPGA Board"><br>
      <em>Target FPGA platform for real-time deployment</em>
    </td>
  </tr>
</table>
</div>

<br>

### [**Urban Displacment Mapping Tool**](https://github.com/tobiassafie/reverse-redlining)
Developed a Python-based data visualization tool to analyze and map patterns of gentrification and economic displacement in Philadelphia. This project combines historical redlining maps with modern census, eviction, and mortgage approval data to reveal how historic inequities persist in housing and income distribution.
<br>
_Conducted independently as an extension of a research paper I wrote for my university's student anthology, **The 33rd**._
<br>
**Tools**: Python, Pandas, GeoPandas, Folium, Plotly, Jupyter
<br>
**Highlights**:
- Integrated datasets from the **HOLC Redlining Maps**, **ACS Census**, and **Eviction Lab**
- Computed tract-level changes in rent, household income, and racial composition
- Built an interactive map overlay showing the correlation between historical red zones and modern eviction or rent-increase hotspots
- Automated data cleaning and geospatial joins using **GeoPandas** and **Folium**
- Designed visual layers for presentation and community engagement
<div align = "center">
<table>
  <tr>
    <td align="center">
      <img src="assets/displacement_map.png" width="400px" alt="Redlining Overlay Map"><br>
      <em>Overlay of historical HOLC redlining zones on current census tracts</em>
    </td>
    <td align="center">
      <img src="assets/rent_change_choropleth.png" width="400px" alt="Eviction Hotspots Map"><br>
      <em>Choropleth of median rent change by census tract</em>
    </td>
  </tr>
</table>
</div>

<br>

### [**GTO Poker Strategy Simulator**](https://github.com/tobiassafie/gto-poker-sim) - _Work in Progress_
Developing a Python-based game-theoretic poker simulator to model optimal mixed strategies under incomplete information. The project applies Monte Carlo simulation and reinforcement-learning methods similar to those used in quantitative finance and algorithmic trading.
<br>
_A fun project I designed to help me learn poker and get a little more competitive than just beating my college game night._
<br>
**Tech:** Python, NumPy, Pandas, Matplotlib, Seaborn
<br>
**Highlights:**
- Implementing hand-bucket abstraction and EV-based decision models  
- Visualizing equilibrium heatmaps and exploitability metrics  
- Experimenting with regret minimization and reinforcement-learning approaches (CFR)  
- Planned extensions: real-time opponent modeling and adaptive counter-strategies

<div align = "center">
<table>
  <tr>
    <td align="center">
      <img src="assets/gto_heatmap.png" width="400px" alt="Redlining Overlay Map"><br>
      <em>Equilibrium betting frequencies across 10 hand buckets in the toy GTO solver, illustrating optimal mixed strategies under balanced play.</em>
    </td>
  </tr>
</table>
</div>

### [**Quantitative Backtester Dashboard**](https://github.com/tobiassafie/quant-backtester)
[**Link to the app**](quantbacktester.streamlit.app)
<br>
Developed an interactive framework for backtesting and visualizing quantitative trading strategies on historical market data. Built using **Streamlit**, the tool allows users to configure parameters, visualize trades, and compare multiple strategy performances in real time. May be recycled in the future to algorithmically trade **event contracts** using **Kalshi's API**.
<br>
_Built independently as a way to familiarize myself with algorithmic trading and ML methods in finance._
**Tech:** Python, Pandas, NumPy, Matplotlib, Streamlit
**Highlights:**
- Modular architecture with five implemented strategies: SMA Crossover, EWMA Crossover, MACD, RSI–Bollinger, and ATR Breakout  
- Integrated analytics for Sharpe Ratio, Sortino Ratio, CAGR, Profit Factor, and Max Drawdown  
- Built interactive overlays for buy/sell markers and indicator signals  
- Designed an extensible structure for adding new strategies and custom metrics  
- Deployed interactive demo using Streamlit Cloud  

<p align="center">
  <img src="assets/MACD_QQQ_PERFORMANCE.png" width="600px" alt="MACD Strategy Performance vs Market"><br>
  <em>Performance of the MACD trading strategy versus a buy-and-hold benchmark, showing cumulative growth, relative outperformance, and daily alpha.</em>
</p>
