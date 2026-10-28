# GenChordProg
Repository for the RLHF Chord Progression system 

Link to website: https://genchordprog.streamlit.app/


File tree:

chord-progression-rl/

├── .gitignore

├── README.md

├── requirements.txt

│

├── data/

│   ├── raw/                         # gitignored

│   │   └── chordonomicon/

│   │       └── chordonomicon_v2.csv

│   │

│   ├── interim/                     # gitignored or optional

│   │   └── chordonomicon_cleaned.parquet

│   │

│   └── processed/                   # small artifacts can be committed

│       ├── chord_vocabulary.json

│       ├── transition_matrix.csv

│       └── chord_sequences.parquet 

│

├── models/                          # trained model artifacts

│   ├── ppo_chord_policy.pt

│   └── reward_model.pt

│

├── notebooks/

│   ├── 01_download_chordonomicon.ipynb

│   ├── 02_clean_chordonomicon.ipynb

│   ├── 03_build_transition_matrix.ipynb

│   ├── 04_train_base_policy.ipynb

│   ├── 05_collect_user_feedback.ipynb

│   ├── 06_train_reward_model.ipynb

│   └── 07_train_ppo_policy.ipynb

│
├── scripts/

│   ├── download_chordonomicon.py

│   ├── clean_chordonomicon.py

│   ├── build_transition_matrix.py

│   └── train_ppo.py

│

├── src/

│   ├── env.py

│   ├── policy.py
│   ├── reward.py
│   └── generation.py
│
└── app/
    └── streamlit_app.py
