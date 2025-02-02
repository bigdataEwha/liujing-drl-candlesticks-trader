# drl-candlesticks-trader
This repository is for the code of paper "Automated Cryptocurrency Trading Approach Using Ensemble Deep Reinforcement Learning: Learn to Understand Candlesticks" which has been submitted to a journal (in review) 

## Abstract (partly)
Despite its high risk, cryptocurrency has gained popularity as a successful trading option. Cryptocurrencies are digital assets that fluctuate dramatically in a market that operates for 24 hours. Developing trading bots using machine learning-based artificial intelligence (AI) approaches has recently received considerable attention. Previous studies have used machine learning techniques to predict financial market trends or make trading decisions, primarily using numeric data extracted from candlesticks. However, these data often ignore the temporal and spatial information present in candlesticks, resulting in a poor understanding of their significance. In this study, we used multi-resolution candlestick images that contain temporal and spatial information on prices. The goal of this study was to compare the performance of raw numeric data and candlestick image data to optimize trading strategies and maximize returns... 

## Image download

Candlesticks image data download: https://drive.google.com/file/d/1qX8K8CRnS3lmhA0Trd1Yk-i7_Cdchwbx/view?usp=sharing  
Copy the unzipped folder "candlesticks" to folder "images"  

## Directories of folders are

-- drl-candlesticks-trader  
&emsp;|  
&emsp;-- code  
&emsp;&emsp;|  
&emsp;&emsp;-- libs  
&emsp;|  
&emsp;-- data  
&emsp;|  
&emsp;-- images  
&emsp;&emsp;|   
&emsp;&emsp;-- candlesticks  
&emsp;|  
&emsp;-- results  
&emsp;&emsp;|  
&emsp;&emsp;-- test  
&emsp;&emsp;&emsp;|  
&emsp;&emsp;&emsp;-- 2022-06-19  
&emsp;&emsp;&emsp;|  
&emsp;&emsp;&emsp;-- 2022-08-15  
&emsp;&emsp;|  
&emsp;&emsp;-- train  
&emsp;&emsp;|  
&emsp;&emsp;-- valid  
&emsp;|  
&emsp;-- runs  
&emsp;|  
&emsp;-- weights  

## Run Example

Train all PPO agents in GPU with multi-resolution raw numerical data  
Type in the terminal: $ python3 code/main.py -t train -g ppo -r multi  

Validate the first DQN agent in GPU with candlestick image  
Type in the terminal: $ python3 code/main.py -t valid -g dqn -f 0 

## License
[MIT](https://choosealicense.com/licenses/mit/)
