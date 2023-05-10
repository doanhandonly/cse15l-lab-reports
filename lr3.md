Grep Command-Lines
=========
1. `grep -l`

      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/fc852e87-13be-4524-ae20-55e24f46469b)
      
      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/e1dd2ba5-de15-4bb5-adc8-92e486f635a5)
      
      When using grep -l, it finds any file path that matches the query, returning all paths that query. Grep -l is extremely useful if you want to find which files contains certain contents, you do not have to 
      open any files one by one, looking for something specific, simply use grep -l (query) and it will point you directly to which file path has what you are looking for. 

2. `grep -iw` (not case-senstive) 

      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/7c17daca-f554-46ca-bde7-3525d64334f2)
      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/40445284-e7c4-43f4-b04c-039d5b166464)
      
      When using grep -iw, it finds lines that contains words matching the command-line input, EXCLUDING SUB-STRINGS. Grep -iw is useful when you want to query for lines that contains the input given in the           command-line, without considering sub-strings. For example, grep -iw "dap" would return a line, "how was your dap", and exclude lines like, "that was daptastic". It is useful when you to really be               specific and "picky" about your query. 
      
3. `grep -n`

      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/cbc0bc76-09cf-43f4-989d-268243456ae2)
      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/44299ab0-883a-49a3-ba7f-8146f15ab385)


