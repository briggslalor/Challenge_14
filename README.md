# Challenge_14

## Algorithmic Trading Model using Machine Learning 

The goal of this project was to build an effective algorithmic trading model for an emrging markets ETF. The goal of the model is to most accurately predict when to buy long or sell short. The trading signals are based off of Standard Moving Average (SMA) calculations over both short and long periods and the times that these cross. With that strategy determined, a number of different supervised machine learning models are trained and tested to see if any could better predict the trading signals. The models tested were the Support Vector Classification (SVC), Linear Regression, Decision Tree Classifier, and AdaBoost Classifier models contained within the Scikit-Learn Module. 

---

## Technologies

This project is built in Python 3.6 and designed to be run in Jupyter Lab. In order to properly utilize the project, the following Python libraries will be used:

   [pandas](https://pandas.pydata.org/docs/)

   [numpy](https://numpy.org/)

   [sklearn](https://scikit-learn.org/stable/)
   
   [hvplot](https://hvplot.holoviz.org/index.html)
   
   [matplotlib](https://matplotlib.org/stable/users/index)


---

## Installation Guide

These additional libraries not included in the base Python can be installed using the pip install syntax. The others are imported within the project file. 

```python
pip install -U scikit-learn
pip install hvplot
```


---

## Usage

Once the proper libraries have been installed into a Python environment, the user can run the project by navigating into the Challenge_14 directory using the command line. When in the directory, the user should open the directory in an instance of Jupyter Lab and run the project. The project will finish running and provide the modeling and analysis of the data. Additional analysis can be found below in the Evaluation Report. 

---

## Evaluation Report

Having completed the analysis within this project, I was able to draw a number of conclusions about the effectiveness of different parameters and machine learning models when building the algorithmic trading model. Given the initial task of building and testing different paramters within the Support Vector Classification Model, I was able to determine the following. 

### Longer Evaluation Periods Produce Better Cumulative Returns

Using the SVC model as a baseline, I tested training periods of 1 month, 3 months, and 6 months. Amongst these different tests, the overall cumulative returns became larger and larger in comparison to the actual returns when the training period was increased. The following graphs show the results. 

[1 Month Training Period](SVC_Window_Testing/svc_returns_comparison_1month_plot.png)

[3 Month Training Period](SVC_Window_Testing/svc_returns_comparison_3month_plot.png)

[6 Month Training Period](SVC_Window_Testing/svc_returns_comparison_6month_plot.png)


---

## Contributors

Briggs Lalor
email: briggsclalor@gmail.com

---

## License

MIT License

Copyright (c) [2021] [Briggs Lalor]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
