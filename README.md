<h1>🔭 Supernova Cosmology Project: Measuring Cosmological Parameters Using Type Ia Supernovae</h1>

<p>This project uses observational data from the Pantheon+SH0ES dataset to measure the Hubble constant (H₀), estimate the age of the Universe, and explore key aspects of cosmic expansion history through Type Ia supernova observations.</p>

<h2>📦 Project Overview</h2>

<ul>
  <li>Plot the Hubble Diagram (Distance Modulus vs. Redshift)</li>
  <li>Fit a Flat ΛCDM Cosmological Model to derive Hubble constant (H₀) and matter density (Ωₘ)</li>
  <li>Estimate the age of the Universe using the fitted parameters</li>
  <li>Analyze residuals to assess model accuracy and identify trends</li>
  <li>Explore results by splitting the dataset into low-redshift and high-redshift subsets</li>
</ul>

<h2>🗂 Dataset</h2>
<p>The project uses the <strong>Pantheon+SH0ES</strong> dataset, containing calibrated distance moduli, redshifts, and uncertainties for Type Ia supernovae. Data is cleaned to exclude rows with missing or invalid values before analysis.</p>

<h2>🛠 Approach and Methodology</h2>

<ol>
  <li><strong>Data Preparation:</strong> Load and clean the Pantheon+SH0ES dataset</li>
  <li><strong>Hubble Diagram:</strong> Plot distance modulus (μ) vs. redshift (z) with logarithmic scaling for clear visualization</li>
  <li><strong>Cosmological Model:</strong> 
    <ul>
      <li>Assume a flat ΛCDM model</li>
      <li>Compute the theoretical distance modulus μ(z, H₀, Ωₘ) using luminosity distance and E(z)</li>
      <li>Fit model to observational data using <code>scipy.optimize.curve_fit</code></li>
    </ul>
  </li>
  <li><strong>Parameter Estimation:</strong> Extract best-fit values and uncertainties for H₀ and Ωₘ</li>
  <li><strong>Age of Universe:</strong> Integrate inverse Hubble parameter to compute cosmic age in Gyr</li>
  <li><strong>Residual Analysis:</strong> Plot residuals (observed - model μ) to check fit quality</li>
  <li><strong>Low-z and High-z Comparison:</strong> Fit subsets of supernovae data to investigate redshift-dependent variations in H₀</li>
</ol>

<h2>📊 Visual Outputs</h2>

<ul>
  <li>Hubble Diagram: μ vs. z with model overlay</li>
  <li>Residual Plot: Residuals vs. redshift to assess fit quality</li>
  <li>Low-z and High-z Hubble constant comparison</li>
</ul>

<h2>🔧 Requirements</h2>
<p>Install dependencies using:</p>

<pre><code>pip install numpy pandas matplotlib scipy astropy</code></pre>

<h2>💡 Insights & Interpretations</h2>

<ul>
  <li>Compare derived H₀ with Planck18 and other literature values</li>
  <li>Estimate Universe's age assuming Ωₘ = 0.3, discuss sensitivity to Ωₘ</li>
  <li>Comment on differences in H₀ for low and high redshift samples</li>
  <li>Discuss assumptions made (flatness, cosmological constant) and potential impacts of relaxing them</li>
</ul>

<h2>🧭 Getting Started</h2>
<p>Clone the repository and run the Jupyter Notebook to reproduce all analysis steps. PDF export of the notebook can be provided for submission or reporting.</p>

<h2>🌌 Scientific Context</h2>
<p>Type Ia supernovae are considered standardizable candles, providing powerful probes for measuring cosmic expansion and dark energy effects. This project follows the modern approach used in observational cosmology to constrain Hubble constant discrepancies and improve understanding of the Universe's history.</p>

<h2>📂 Repository Contents</h2>

<ul>
  <li><code>Pantheon+SH0ES.txt</code> — Supernova dataset </li>
  <li><code>supernova_cosmology.ipynb</code> — Complete analysis notebook</li>
  <li><code>README.md</code> — Project overview and instructions</li>
  <li><code>requirements.txt</code> — List of required Python packages</li>
</ul>
