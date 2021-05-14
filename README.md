# NFL Top Players Analysis
The goal of this case study is to read in the Fantasy Football information we have gathered in order to determine the best player at certain positions every year (1999 - 2019) in the NFL.

Our strategy is to use Fantasy Points as a basis for individual performance. However, a major part will be instead of just judging players soley on how many points they gain in a season we will also be looking at how good their opponent's defense was against their position.

Firstly we will read in the fantasy data, cleaning it and adding the different opponents to the data from a schedule file. We will then remove the outliers from the data before finding average performance by position through the years. We will find the average using EMA. We will then find the average yearly performance of each team's defense against the 5 positions we are tracking for each individual year. To normalize our data we will be taking the difference between the opponent team's average fantasy points given up and the positons EMA for that year. That difference will give us our Adjusted Points Value. A players Adjusted Point value will be totaled for the entire season, the player with the highest total Adjusted Points for the year at their position will be determined the top preformer.

## Install
The project is setup and can be run through any Jupyter Notebook server.

## Dependencies
  * Numpy
  * Pandas
  * Scipy
  
## License

Copyright 2021 James Denbow

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
