# **Sunlight Network \- Data Format Guide**

All individual data files are stored in the people/ directory.

## **Data Fields**

| Field | Type | Required | Description |
| :---- | :---- | :---- | :---- |
| id | String | **Yes** | Unique identifier (e.g. "1", "aviv\_geffen"). |
| name | String | **Yes** | Full display name. |
| updatedAt | Date String | No | Format: YYYY-MM-DD. Date of last update. |
| description | String | **Yes** | Bio. **Use \#tags here\!** (e.g., \#developer \#israel). |
| photo | String (URL) | No | Direct image URL. |
| positions | Array\<String\> | No | List of roles. |
| links | Array\<Object\> | No | Connections to others. |

## **Tags**

Add tags directly in the description field using \#.  
Example: "Senior \#developer living in \#TelAviv"

## **Links Object**

{  
  "targetId": "other-person-id",  
  "updatedAt": "2023-11-20",  
  "description": "Worked together at Google",  
  "referenceUrl": "https://..."  
}  
