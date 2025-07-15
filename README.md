# English-German-Dutch-political-statements-model
Model trained on recent political platforms for the USA, Germany, the Netherlands, and Belgium/Flanders

# Training Summary Report

**Generated:** 2025-07-08 13:36:36

---

## 📊 HYBRID MODEL TRAINING SUMMARY REPORT

### 📁 Dataset Composition

- **📈 Training samples:** 383
- **📉 Test samples:** 95
- **📊 Total samples:** 478
- **⚓ Prototype anchors:** 9
- **📝 Real texts:** 374
- **📄 Original texts:** 374
- **🔄 Paraphrased texts:** 0
- **📈 Augmentation ratio:** 0.0x

#### 📂 Files Processed

| File | Original Texts | Paraphrased Texts | Total | Augmentation |
|------|:--------------:|:-----------------:|:-----:|:------------:|
| `AllHumanGoalRatings2012_reliable.csv` | 50 | 0 | 50 | 0.0x |
| `AllHumanGoalRatingsBE_reliable.csv` | 38 | 0 | 38 | 0.0x |
| `AllHumanGoalRatingsGerman_reliable.csv` | 70 | 0 | 70 | 0.0x |
| `AllHumanGoalRatingsManifesto_reliable_clean.csv` | 86 | 0 | 86 | 0.0x |
| `AllHumanGoalRatingsNL_reliable.csv` | 64 | 0 | 64 | 0.0x |
| `AllHumanGoalRatingsSpeaches_reliable.csv` | 66 | 0 | 66 | 0.0x |

#### 🎯 Goal Type Distributions

| Type | Mean | Std | Range |
|------|:----:|:---:|:-----:|
| **📊 Prog** | 0.734 | 0.175 | [0.143, 1.000] |
| **📊 Mant** | 0.485 | 0.175 | [0.171, 1.000] |
| **📊 Prot** | 0.602 | 0.187 | [0.143, 0.971] |

---

## 🏗️ Model Status

- **🧠 Total parameters:** 280,011,267
- **🔧 Trainable parameters:** 280,011,267
- **📐 Model size:** ~1068.2 MB
- **✅ Status:** Model is loaded and ready

### 🔧 Configuration

```yaml
embedding_models: ['paraphrase-multilingual-mpnet-base-v2']
hidden_layers: [256]
use_attention: true
paraphrase_rounds: 0
epochs: 20
batch_size: 32
learning_rate: 0.001
dropout_rate: 0.2
trainable_embeddings: true
batch_norm: true
attention_heads: 1
```

---

## 📈 Model Performance

### 📊 Overall Test Correlations

| Goal Type | Correlation |
|-----------|:-----------:|
| 🎯 **Progressive** | 0.433 |
| ⚖️ **Maintenance** | 0.545 |
| 🛡️ **Protective** | 0.567 |
| 📈 **Average** | **0.515** |

### 📂 Correlations by Source

| Source File | Samples | Progressive | Maintenance | Protective | Average |
|-------------|:-------:|:-----------:|:-----------:|:----------:|:-------:|
| `AllHumanGoalRatings2012_reliable.csv` | 13 | 0.770 | 0.701 | 0.673 | **0.715** |
| `AllHumanGoalRatingsBE_reliable.csv` | 10 | 0.644 | 0.481 | 0.545 | 0.556 |
| `AllHumanGoalRatingsGerman_reliable.csv` | 17 | 0.305 | 0.687 | 0.812 | 0.601 |
| `AllHumanGoalRatingsManifesto_reliable_clean.csv` | 22 | 0.022 | 0.333 | 0.406 | 0.254 |
| `AllHumanGoalRatingsNL_reliable.csv` | 16 | 0.662 | 0.688 | 0.637 | 0.662 |
| `AllHumanGoalRatingsSpeaches_reliable.csv` | 17 | 0.175 | 0.457 | 0.630 | 0.421 |

### 📊 Correlation Summary

- **🏆 Best overall performance:** AllHumanGoalRatings2012_reliable.csv (0.715)
- **⚠️ Worst overall performance:** AllHumanGoalRatingsManifesto_reliable_clean.csv (0.254)
- **Progressive correlations:** 0.430 ± 0.304
- **Maintenance correlations:** 0.558 ± 0.155
- **Protective correlations:** 0.617 ± 0.135

### 📏 Prediction Errors (Mean Absolute Error)

| Goal Type | MAE | Std Dev |
|-----------|:---:|:-------:|
| Progressive | 0.167 | ± 0.120 |
| Maintenance | 0.107 | ± 0.081 |
| Protective | 0.125 | ± 0.103 |
