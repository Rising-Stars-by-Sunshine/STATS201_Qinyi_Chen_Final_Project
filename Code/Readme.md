# Data Query and Data Analysis Process
## Data Query
This project investigates the correlation between personality traits and cognitive biases using data from [Wolfram Cloud's dataset on Cognitive Biases and Mindfulness](https://datarepository.wolframcloud.com/resources/Philip%20Z.%20Maymin_Data-for-Maymin--Langer-2021-Cognitive-Biases-and-Mindfulness/). The process begins with loading the dataset, followed by renaming specific columns for clarity and quantifying the variables to ensure compatibility with machine learning algorithms. The data is then analyzed using various machine learning models to identify significant predictors and their relationships.

## Pseudo-code
```
\begin{table}[h]
\centering
\begin{tabular}{|c|l|}
\hline
\textbf{Step} & \textbf{Pseudo-code} \\ \hline
1 & Load\_Data(``URL'') \\ \hline
2 & Rename\_Columns(``old\_name1'', ``new\_name1'') \\ \hline
3 & Quantify\_Variables(``column\_names'') \\ \hline
4 & Split\_Data(``train\_size=0.7, test\_size=0.3'') \\ \hline
5 & Train\_Model(``model\_type'', ``parameters'') \\ \hline
6 & Evaluate\_Model(``metrics'') \\ \hline
7 & Visualize\_Results(``type\_of\_plot'') \\ \hline
\end{tabular}
\caption{Pseudo-code for data query and analysis applicable in Python, Java, and Go.}
\label{tab:pseudocode}
\end{table}
```
[Markmap_of_Data_Query_and_Analysis](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/edit/main/Code/mark_code.png)
