# RS-GCL
This is the PyTorch implementation for RS-GCL proposed in the paper.


### 1. Note on datasets
Due to the large size of datasets *ML-10M*, *Amazon* and *Tmall*, we have compressed them into zip files. Please unzip them before running the model on these datasets. For *Yelp* and *Gowalla*, keeping the current directory structure is fine.



### 2. Running environment

We develope our codes in the following environment:

```
Python version 3.9.12
torch==1.12.0+cu113
numpy==1.21.5
tqdm==4.64.0
```

### 3. How to run the codes

* Yelp
```
python main.py --data yelp
```

* Gowalla

```
python main.py --data gowalla --lambda2 1e-5 --temp 0.3
```

* ML-10M

```
python main.py --data ml10m --temp 10
```

* Amazon

```
python main.py --data amazon --lambda1 1e-5 --temp 0.1
```

* Tmall

```
python main.py --data tmall --lambda1 1e-6 --temp 0.3 --dropout 0
```




