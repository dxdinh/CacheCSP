### Query list of testspec in the system
```
Select  ad.Name,  ts.* from stats.testspec ts
 JOIN Codelist.AnalyteDescription ad ON ts.Analyte = ad.Analyte and languageKey = 'en'
 ```
 
 
### Query distinct analyte in use by testspec
```
Select DISTINCT ad.Analyte as analyteID , ad.Name from stats.testspec ts
 JOIN Codelist.AnalyteDescription ad ON ts.Analyte = ad.Analyte and languageKey = 'en'
```

### Query list of Analyte
```
Select DISTINCT tb1.Analyte as analyteID , tb1.Name AnalyteName from Codelist.AnalyteDescription tb1 where  tb1.languageKey = 'en'
```
