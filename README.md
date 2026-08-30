# EOT2D-MASLD Predictor

A freely accessible, single-file web calculator for estimating the risk of metabolic dysfunction-associated steatotic liver disease (MASLD) in patients with early-onset type 2 diabetes mellitus (EOT2D).

**Online calculator:** https://syzh1.github.io/EOT2D-MASLD-Predictor/

## Model

The calculator is powered by a 12-variable extreme gradient boosting (XGB) model:

- BMI
- Alcohol drinking
- HDL-C
- ALT
- Total protein (TP)
- Indirect bilirubin (IBIL)
- Uric acid (UA)
- Albumin (ALB)
- Globulin (GLO)
- Metformin use
- Acarbose use
- ALT/AST ratio

For each patient, the tool returns the predicted probability of MASLD, a risk stratification (low / moderate / high), the model decision at the Youden-optimised cutoff (0.668), and per-variable SHAP contributions.

Internal test performance: AUROC 0.759 (n = 397).

## Usage

- **Online:** open the calculator link above in any modern browser (no installation required).
- **Offline:** download `index.html` and double-click it; the page runs entirely in the browser with no server or internet connection.

## Disclaimer

This tool is provided for research purposes only and is not a substitute for clinical judgement.

## Citation

If you use this tool, please cite the associated manuscript (DOI to be added upon publication).

## License

MIT
