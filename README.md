# Stock-Price-Prediction-with-RNN-


**Train a model only on SP500.csv; no embedding**

python main.py --stock_symbol=SP500 --train --input_size=1 --lstm_size=128 --max_epoch=50

**Train a model on 100 stocks; with embedding of size 8**

python main.py --stock_count=100 --train --input_size=1 --lstm_size=128 --max_epoch=50 --embed_size=8

**Start your Tensorboard**

cd stock-rnn
mkdir logs
tensorboard --logdir ./logs --port 1234 --debug

**My python environment:**

Python version == 2.7
BeautifulSoup==3.2.1
numpy==1.13.1
pandas==0.16.2
scikit-learn==0.16.1
scipy==0.19.1
tensorflow==1.2.1
urllib3==1.8
