# Project 2: Enrique Briceno, Thomas Guyton, Erik McFarlane

## Methodology:
<ul>
  <li>Select three stocks based on volatility (High, Avg, & Low as measured by the stock’s Beta)
  <li>Select three different trading indicators (MACD, Commodity Channel Indicator (CCI), and Money Flow Index (MFI)
  <li>Apply two different ML libraries (SVC & LTSM) to attempt to predict stock prices and indicators based off of those indicators and to see if different indicators work better for different classes of stocks (based on volatility)
</ul>

## Results:
MACD: 
  <ul>
    <li>![Alt text](https://github.com/e-mcfarlane/project-2/blob/main/cat-macd.jpg "CAT MACD results")
    <li>![Alt text](https://github.com/e-mcfarlane/project-2/blob/main/ostk-macd.jpg "OSTK MACD results")
    <li>![Alt text](https://github.com/e-mcfarlane/project-2/blob/main/dgx-macd.jpg "DGX MACD results")
  </ul>
  CCI & MFI: 
  <ul>
    <li>![Alt text](https://github.com/e-mcfarlane/project-2/blob/main/cat-cci-mfi.jpg "CAT CCI & MFI results")
    <li>![Alt text](https://github.com/e-mcfarlane/project-2/blob/main/ostk-cci-mfi.jpg "OSTK CCI & MFI results")
    <li>![Alt text](https://github.com/e-mcfarlane/project-2/blob/main/dgx-cci-mfi.jpg "DGX CCI & MFI results")
  </ul>


## Conclusions
<ul>
  <li>Using LSTM on the indicator to predict the CLOSE price was very poor across the board, generally failed to capture big increases or decreases in price and stayed in a narrow band
  <li>Using LSTM on the indicator to predict the INDICATOR was much better, however, still trailed actual values and yielded much worse returns
  <li>There were no trends as to whether a model did better with a more or less volatile stock (low sample size
  <li>Models used were better at predicting simplistic, binary “Buy/Sell” (i.e. MACD) based on indicators versus multi-variable or trend change (e.g. from Buy to Sell, Buy to Hold, Hold to Sell, etc)
