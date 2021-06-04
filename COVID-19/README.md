*COVID-19 Data*
==========  

*최종 matplotlib 결과물*
-----
<img src="https://user-images.githubusercontent.com/66001539/120742822-a27bef80-c532-11eb-9e2d-df1ec3c18f68.png" width="450px" height="450px" title="px(픽셀) 크기 설정" alt="Image_machine"></img><br/>  


*전체 출력*
-----  
>
                Country      Continent          Last_Update        Lat       Long_  Confirmed  Deaths  Recovered  Active  Incident_Rate
0             Australia      Australia  2020-08-10 06:34:52 -25.000000  133.000000    21397.0   313.0    12141.0  8943.0      84.042624
1               Austria         Europe  2020-08-10 06:34:52  47.516200   14.550100    22033.0   721.0    19923.0  1389.0     244.637147
2                Canada  North America  2020-08-10 06:34:52  60.001000  -95.001000   121367.0  9028.0   105420.0  6919.0     320.604278
3                 China           Asia  2020-08-10 06:34:52  30.592800  114.305500    88793.0  4686.0    82125.0  1982.0       6.321243
4               Denmark         Europe  2020-08-10 06:34:52  56.263900    9.501800    14759.0   617.0    13069.0  1073.0     254.808058
..                  ...            ...                  ...        ...         ...        ...     ...        ...     ...            ...
183  West Bank and Gaza         Others  2020-08-10 06:34:52  31.952200   35.233200    14208.0    97.0     7945.0  6166.0     278.510908
184      Western Sahara         Others  2020-08-10 06:34:52  24.215500  -12.885800       10.0     1.0        8.0     1.0       1.674116
185               Yemen           Asia  2020-08-10 06:34:52  15.552727   48.516388     1804.0   515.0      913.0   376.0       6.048421
186              Zambia         Africa  2020-08-10 06:34:52 -13.133897   27.849332     8085.0   235.0     6698.0  1152.0      43.978565
187            Zimbabwe         Africa  2020-08-10 06:34:52 -19.015438   29.154857     4649.0   104.0     1437.0  3108.0      31.279169
  
*나라, 확진자, 사망자 데이터만 추출*
-----  
>
[188 rows x 10 columns]
                    Confirmed  Deaths
Country                              
Australia             21397.0   313.0
Austria               22033.0   721.0
Canada               121367.0  9028.0
China                 88793.0  4686.0
Denmark               14759.0   617.0
...                       ...     ...
West Bank and Gaza    14208.0    97.0
Western Sahara           10.0     1.0
Yemen                  1804.0   515.0
Zambia                 8085.0   235.0
Zimbabwe               4649.0   104.0
  

*# 나라별 사망률 구하기*
-----  
> [188 rows x 2 columns]  
                    Confirmed  Deaths  Death Rate (Per 100)
Country                                                    
Australia             21397.0   313.0              1.462822
Austria               22033.0   721.0              3.272364
Canada               121367.0  9028.0              7.438595
China                 88793.0  4686.0              5.277443
Denmark               14759.0   617.0              4.180500
...                       ...     ...                   ...
West Bank and Gaza    14208.0    97.0              0.682714
Western Sahara           10.0     1.0             10.000000
Yemen                  1804.0   515.0             28.547672
Zambia                 8085.0   235.0              2.906617
Zimbabwe               4649.0   104.0              2.237040
  

*사망률 가장 높은 10개 나라 (사망자 1000명 이상)*
-----  
[188 rows x 3 columns]
             Confirmed   Deaths  Death Rate (Per 100)
Country                                              
Ireland        26712.0   1772.0              6.633723
Sweden         82323.0   5763.0              7.000474
Canada        121367.0   9028.0              7.438595
Spain         314362.0  28503.0              9.066936
Netherlands    59360.0   6178.0             10.407682
Mexico        480278.0  52298.0             10.889110
France        235237.0  30327.0             12.892105
Belgium        74152.0   9872.0             13.313195
Italy         250566.0  35205.0             14.050190
UK            312574.0  46659.0             14.927345
