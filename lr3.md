Grep Command-Lines
=========
1. `grep -l`

      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/fc852e87-13be-4524-ae20-55e24f46469b)
      
      (Used grep -l to find the path that match and contains my query, in this case, it is "beach") 
      
      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/e1dd2ba5-de15-4bb5-adc8-92e486f635a5)
      
      (Used grep -l on a directory, government/, it returns all the possiblt path within this directory) 
      
      When using grep -l, it finds any file path that matches the query, returning all paths that query. Grep -l is extremely useful if you want to find which files contains certain contents, you do not have to 
      open any files one by one, looking for something specific, simply use grep -l (query) and it will point you directly to which file path has what you are looking for. 

2. `grep -iw` 

      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/7c17daca-f554-46ca-bde7-3525d64334f2)
      
      (Used grep -iw, to locate files that match the given in-line arguement. in this case being, "dap")
      
      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/40445284-e7c4-43f4-b04c-039d5b166464)
      
      (Used grep -iw, to locate files that match the given in-line arguement. in this case being, "beach")

      When using grep -iw, it finds lines that contains words matching the command-line input, EXCLUDING SUB-STRINGS. Grep -iw is useful when you want to query for lines that contains the input given in the           command-line, without considering sub-strings. For example, grep -iw "dap" would return a line, "how was your dap", and exclude lines like, "that was daptastic". It is useful when you to really be               specific and "picky" about your query. 
      
3. `grep -n`

      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/cbc0bc76-09cf-43f4-989d-268243456ae2)
      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/44299ab0-883a-49a3-ba7f-8146f15ab385)
      
      Grep -n returns the files that contains the command-line input, and returns the exact line in that file that contains that character. Like grep -l, it locates which files contains your input query. On top       of that, it also returns the line in which it is situated. If you ever need to reference which line number contains said query, then grep -n can do just that. 

4. `grep -e`
      
      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/4509ebbc-5766-4531-8817-5748eba5b07d)
      ![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/c668f391-ea88-485d-b3e0-d820d8d51013)

      Grep -e grants the ability to query/ search for multiple command-line inputs, returning the lines and file path that matches the multiple searches. Grep -e is extremely useful when you want to save time         who doesn't want to save time. By allowing you to search/query multiple inputs instead of one, you can do all your searching in one input. 

      
# **Sources**
1. ChatGPT
2. `git grep --help` - pulls up a mini documentation manual of grep commands
3. https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/
