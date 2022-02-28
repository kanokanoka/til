# Banditは何

参考  
https://bandit.readthedocs.io/en/latest/

Pythonコードのscanができる（はず)

Getting Started  
https://bandit.readthedocs.io/en/latest/start.html

pip3で入れるだけ

bandit -r path/to/your/codeする。 a.pyとかでいい

    (env1_bandit) [root@ip-172-31-2-99 gomi]# bandit -r a.py 
    [main]	INFO	profile include tests: None
    [main]	INFO	profile exclude tests: None
    [main]	INFO	cli include tests: None
    [main]	INFO	cli exclude tests: None
    [main]	INFO	running on Python 3.7.4
    [node_visitor]	WARNING	Unable to find qualified name for module: a.py
    Run started:2022-02-28 12:43:58.181076
    
    Test results:
    	No issues identified.
    
    Code scanned:
    	Total lines of code: 2
    	Total lines skipped (#nosec): 0
    
    Run metrics:
    	Total issues (by severity):
    		Undefined: 0
    		Low: 0
    		Medium: 0
    		High: 0
    	Total issues (by confidence):
    		Undefined: 0
    		Low: 0
    		Medium: 0
    		High: 0
    Files skipped (0):
