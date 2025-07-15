# English-German-Dutch-political-statements-model
Model trained on recent political platforms for the USA, Germany, the Netherlands, and Belgium/Flanders

Training Summary Report
Generated: 2025-07-08 13:36:36
================================================================================

================================================================================
📊 HYBRID MODEL TRAINING SUMMARY REPORT
================================================================================

📁 DATASET COMPOSITION
----------------------------------------
📈 Training samples: 383
📉 Test samples: 95
📊 Total samples: 478
⚓ Prototype anchors: 9
📝 Real texts: 374
📄 Original texts: 374
🔄 Paraphrased texts: 0
📈 Augmentation ratio: 0.0x

📂 FILES PROCESSED:
  📄 AllHumanGoalRatings2012_reliable.csv
     • Original texts: 50
     • Paraphrased texts: 0
     • Total from source: 50
     • Augmentation: 0.0x
  📄 AllHumanGoalRatingsBE_reliable.csv
     • Original texts: 38
     • Paraphrased texts: 0
     • Total from source: 38
     • Augmentation: 0.0x
  📄 AllHumanGoalRatingsGerman_reliable.csv
     • Original texts: 70
     • Paraphrased texts: 0
     • Total from source: 70
     • Augmentation: 0.0x
  📄 AllHumanGoalRatingsManifesto_reliable_clean.csv
     • Original texts: 86
     • Paraphrased texts: 0
     • Total from source: 86
     • Augmentation: 0.0x
  📄 AllHumanGoalRatingsNL_reliable.csv
     • Original texts: 64
     • Paraphrased texts: 0
     • Total from source: 64
     • Augmentation: 0.0x
  📄 AllHumanGoalRatingsSpeaches_reliable.csv
     • Original texts: 66
     • Paraphrased texts: 0
     • Total from source: 66
     • Augmentation: 0.0x

🎯 GOAL TYPE DISTRIBUTIONS:
  📊 Prog:
     • Mean: 0.734
     • Std:  0.175
     • Range: [0.143, 1.000]
  📊 Mant:
     • Mean: 0.485
     • Std:  0.175
     • Range: [0.171, 1.000]
  📊 Prot:
     • Mean: 0.602
     • Std:  0.187
     • Range: [0.143, 0.971]

🏗️  MODEL STATUS
----------------------------------------
🧠 Total parameters: 280,011,267
🔧 Trainable parameters: 280,011,267
📐 Model size: ~1068.2 MB
✅ Model is loaded and ready

🔧 CONFIGURATION:
  • embedding_models: ['paraphrase-multilingual-mpnet-base-v2']
  • hidden_layers: [256]
  • use_attention: True
  • paraphrase_rounds: 0
  • epochs: 20
  • batch_size: 32
  • learning_rate: 0.001
  • dropout_rate: 0.2
  • trainable_embeddings: True
  • batch_norm: True
  • attention_heads: 1

📈 MODEL PERFORMANCE
----------------------------------------
🔮 Generating predictions on test set...

📊 OVERALL TEST CORRELATIONS:
  🎯 Progressive: 0.433
  ⚖️  Maintenance: 0.545
  🛡️  Protective:  0.567
  📈 Average:     0.515

📂 CORRELATIONS BY SOURCE:
-----------------------------------
📄 AllHumanGoalRatings2012_reliable.csv
   Samples: 13
   Progressive: 0.770
   Maintenance: 0.701
   Protective:  0.673
   Average:     0.715

📄 AllHumanGoalRatingsBE_reliable.csv
   Samples: 10
   Progressive: 0.644
   Maintenance: 0.481
   Protective:  0.545
   Average:     0.556

📄 AllHumanGoalRatingsGerman_reliable.csv
   Samples: 17
   Progressive: 0.305
   Maintenance: 0.687
   Protective:  0.812
   Average:     0.601

📄 AllHumanGoalRatingsManifesto_reliable_cl...
   Samples: 22
   Progressive: 0.022
   Maintenance: 0.333
   Protective:  0.406
   Average:     0.254

📄 AllHumanGoalRatingsNL_reliable.csv
   Samples: 16
   Progressive: 0.662
   Maintenance: 0.688
   Protective:  0.637
   Average:     0.662

📄 AllHumanGoalRatingsSpeaches_reliable.csv
   Samples: 17
   Progressive: 0.175
   Maintenance: 0.457
   Protective:  0.630
   Average:     0.421

📊 CORRELATION SUMMARY:
   Best overall performance: AllHumanGoalRatings2012_reliab... (0.715)
   Worst overall performance: AllHumanGoalRatingsManifesto_r... (0.254)
   Progressive correlations: 0.430 ± 0.304
   Maintenance correlations: 0.558 ± 0.155
   Protective correlations:  0.617 ± 0.135

📏 PREDICTION ERRORS (Mean Absolute Error):
   Progressive: 0.167 ± 0.120
   Maintenance: 0.107 ± 0.081
   Protective:  0.125 ± 0.103

================================================================================

