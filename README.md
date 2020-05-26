### goex_backtest 基于orderbook数字货币回测
#### 回测数据格式说明
1.标准的csv格式文件，注意：不需要header     
2.模版如下:    
 
 | timestamp | ask[n].price | ask[n].amount | ... | ask[0].price | ask[0].amount | bid[0].price | bid[0].amount | ... | bid[n].price | bid[n].amount |
 | --------- | ------------ | ------------- | --- | ------------ | ------------- | ------------ | ------------- | --- | ------------ | ------------- |
 | 1569888000143 | 8000.1 | 0.34 | ... | 7800.5 | 1.20 | 8000 | 0.15 | ... | 7700.2 | 12.002 |

3. 第一列时间戳精确到`毫秒` , 卖单降序排列，买单升序排列.       
4. 支持任意档数的深度回测，只需要设置对应的参数。    
  

  