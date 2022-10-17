# AMOS22_solutions ouradiology


This repository shows how to use our docker image of our solutions in Multi-Modality Abdominal Multi-Organ Segmentation Challenge (AMOS22).
Our team achieved 2nd place in task1 and 3rd place in task2 in final test phase. The final ranking leaderboard is [here](https://amos22.grand-challenge.org/final-ranking/).

We referred to [official github](https://github.com/JiYuanFeng/AMOS/tree/docker) to make docker images. In order to predict images, just use the following command;

```
docker run --rm --runtime=nvidia --ipc=host  -e NVIDIA_VISIBLE_DEVICES=all --gpus 0 --user root -v LOCAL_PATH_INPUT:/workspace/input/:ro -v LOCAL_PATH_OUTPUT:/workspace/output/ TEAMNAME python run_inference.py
```

Both docker images in task1 and task2 is uploaded in [google drive](https://drive.google.com/drive/folders/1plS5nNRIF2fNZm-BxjiTckF9JNFEUbp8?usp=sharing).

Our method and experimental results are summerized arxiv.  
If you have questions, feel free to ask me.