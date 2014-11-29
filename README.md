pyligadb
========
A Python wrapper for the OpenLigaDB webservice.

OpenLigaDB is a german SOAP webservice providing sports results and scores, especially from german soccer leagues. See http://www.openligadb.de for more information.

###Example use:

```python
from pyligadb.pyligadb import API
api = API()
matches = api.getMatchdataByGroupLeagueSaison(14, 'bl1', 2010)
for match in matches:
    print "%s vs. %s" % (match.nameTeam1, match.nameTeam2)
```
Result:
```
1. FSV Mainz 05 vs. 1. FC Nuernberg
1899 Hoffenheim vs. Bayer Leverkusen
...
...
```

Take a look at the code for all available functions or see the original documentation here: http://www.openligadb.de/Webservices/Sportsdata.asmx
