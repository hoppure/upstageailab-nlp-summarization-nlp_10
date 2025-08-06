# Summary DL pipeline for NLP competition

## For Upstage NLP competition

### Dataset
Upstage NLP competition dataset(dialogue summarization)

### Quick setup

```bash
# clone project
git clone https://github.com/ohseungtae/upstageailab-nlp-summarization-nlp_10.git
cd upstageailab-nlp-summarization-nlp_10




# install requirements
pip install -r requirements.txt
```

### Model Hyper-Parameters Tuning

* end-to-end
```shell
python main.py mode=tune is_tuned=untuned num_trials={num_trials}
```

### Training

* end-to-end
```shell
python main.py mode=train is_tuned={tuned or untuned} num_trials={num_trials}
```

### Test

* end-to-end
```shell
python main.py mode=test is_tuned={tuned or untuned} num_trials={num_trials} epoch={ckpt epoch}
```

### Prediction

* end-to-end
```shell
python main.py mode=predict is_tuned={tuned or untuned} num_trials={num_trials} epoch={ckpt epoch}
```


__If you want to change main config, use --config-name={config_name}.__

__Also, you can use --multirun option.__

__You can set additional arguments through the command line.__
