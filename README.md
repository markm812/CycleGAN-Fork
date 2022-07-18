Personal copy of Repo: https://github.com/jackaduma/CycleGAN-VC2  

Clone voice only:  

python train.py --logf0s_normalization ./cache/logf0s_normalization.npz --mcep_normalization ./cache/mcep_normalization.npz --coded_sps_A_norm ./cache/coded_sps_A_norm.pickle --coded_sps_B_norm ./cache/coded_sps_B_norm.pickle --model_checkpoint ./model_checkpoint/ --resume_training_at ./model_checkpoint/_CycleGAN_CheckPoint --validation_A_dir ./data/valid_A/ --output_A_dir ./converted_sound/valid_A --validation_B_dir ./data/valid_B/ --output_B_dir ./converted_sound/valid_B --vc_only True  

Training:
python train.py --logf0s_normalization ./cache/logf0s_normalization.npz --mcep_normalization ./cache/mcep_normalization.npz --coded_sps_A_norm ./cache/coded_sps_A_norm.pickle --coded_sps_B_norm ./cache/coded_sps_B_norm.pickle --model_checkpoint ./model_checkpoint/ --resume_training_at ./model_checkpoint/_CycleGAN_CheckPoint --validation_A_dir ./data/valid_A/ --output_A_dir ./converted_sound/valid_A --validation_B_dir ./data/valid_B/ --output_B_dir ./converted_sound/valid_B 

Preprocess:
python preprocess_training.py --train_A_dir ./data/clean/ --train_B_dir ./data/tts_audio/ --cache_folder ./cache/