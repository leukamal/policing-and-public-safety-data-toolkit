# Police Stops Data Dictionary

### Standard fields
| Field | Data Type | Description | Length | Expected Pattern | null? |  
| ----- | ---- | ---- | ---- | ---- |---- |  
| stop_date | datetime | The date and time when the stop occurred. | 19 | YYYY/MM/DD HH24:MM:SS |no |  
| subject_race | string | Reported race of the person being stopped. | varies | varies, 'Unknown' | yes |  
| subject_sex | string | Gender of person being stopped. | varies | ('Male', 'Female', 'Non-Binary', 'Unknown' | yes |  
| subject_age | integer | Age of person being stopped. | 3 | [10-150] | yes |  
| search_conducted | string | Was a vehicle searched? | 1 | ('y','n','u') | yes |  
| contraband_found | string | Was contraband found in the search or frisk? | 1 | ('y','n','u') | yes |  
| citation_issued | string | Was a citation issued? | 1 | ('y','n','u') | yes |  
| warning_issued | string | Was a warning issued? | 1 | ('y','n','u') | yes |  
| frisk_performed | string | Was a body search performed? | 1 | ('y','n','u') | yes |  
| arrest_made | string | Was the person being stopped arrested? | 1 | ('y','n','u') | yes |  
| reason_for_stop | string | What was the reasong for the stop? | varies | varies, 'Unknown' | yes |  

### Extended fields
| Field | Data Type | Description | Length | Expected Pattern | null? |  
| ----- | ---- | ---- | ---- | ---- |---- |  
| stop_latitude | string | Latitude of where the stop occurred. | 9-10 | DDD MM SS('N','S','E','W') |---- |  
| stop_longitude | string | Longitude of where the stop occurred. | 9-10 | DDD MM SS('N','S','E','W') |---- |  