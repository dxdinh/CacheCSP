### Query list of testspec in the system
```
Select  ad.Name,  ts.* from stats.testspec ts
 JOIN Codelist.AnalyteDescription ad ON ts.Analyte = ad.Analyte and languageKey = 'en'
 ```
 
 
