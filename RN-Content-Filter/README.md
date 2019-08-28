# Content Filter

*Built by LATAM Team*

**Supports:** *iOS and Android*
*Current Version: 1.0.6*

 
## About

The content filter is main to address a basic filtering of content in an app.

## What needs does it meet?
### Simulate a simple search
The filter acts as a simple search for content. Although is a simple solution this plugin can help a user to quickly traverse through content.


### When to use?

- The catalog is if a small quantity.
- The client wants to facilitate the action of finding content for familiarized users.
- The client does not have a robust backend search engine.
- The client does not care about analytics and data gathered through a search engine.

## Analytics

- None at the moment. The product should consider the following event:
  - Selected content

## Related Technologies

- The product should evolve into an integration with cliud based solutions. 

## Configuration

### Feed Structure

Here you can find in detail manner the fields and data necessary to build the specific structure. Keep in mind this structure will define an EPG for single or multiple live channels or live events.

Parameter | Description | Type
---------|----------|---------
 |**type** | An object containing a value. This used to give meaning to this section. | **Object**|
 ||-**value** : A **string** that references the use for this Json response. For this context “feed” shall be the value." ||
 |**title** |	A string to describe the feed.	| **String**|
 |**entry**|	List of entry Object defining the program schedule for an specific channel or live event.	|**Object**|
 |**extensions**	|An object to specify custom key/value pairs or json objects. Refer to extensions Object.	|**Object**|

### Entry Object

Parameter | Description | Type
---------|----------|---------
 |**type** | - An object containing a value. This used to give meaning to this section. **value** : A string that references the use for this json response. For this context “feed” shall be the value.  | **Object**|
 ||- **value** : A **string** that references the use for this json response. For this context “**feed**” shall be the value.|
 |**id** | A numeric incremental value to identify the entry object. | **Integer**|
 |**title** | String for the content title | **String**|   
 |**summary** | A string with a brief description of the program. | **String**|
 |**published** | Timestamp stating the time the content was published. Format *YYYY-MM-DDThh:mm:ss—hhmm*. | **String**|
 |**updated** | Timestamp stating the last time the content was updated. Format *YYYY-MM-DDThh:mm:ss—hhmm*. | **String**| 
 |**author** | String to define add the author of the media type in place. | **String**|
 |**media_group** | An object that can contain different types of media item objects.| **Object**|
 ||- **type** : Indicates how the media_item object should be treated. For this context “image” shall be used. This image will graphically reference the video content.||
 ||- **media_item** : refer to media_item Object.||
 |**content** | An object that can be used to defined the media referenced by the entry.| **Object**|
 ||- **type** : Indicates the type of media content is referenced by the entry. For this context **“feed”** shall be used.||
 ||- **src** : A **url string** referencing the media asset source.||
 |**link** | An object that can be used to define an alternate link to the content.| **Object**|
 ||- **rel** : Indicates the action to take place, for this particular use “self” should be the value.||
 ||- **type** : Indicates the type of media content is referenced by the entry. For this context **“feed”** shall be used.||
 ||- **src** : A **url string** referencing the the link.||
 

 ### Media_item Object

Parameter | Description | Type
---------|----------|---------
 |**src** | A **url string** referencing to the media asset source. | **String**|
 |**key** | A **string** to identify among other the media_item objects.  | **String**|
 |**type** | A **string** to define the kind of media asset. | **Object**|


## Feed Example
```
    {
 "type": {
   "value": "feed"
 },
 "title": "FEED TITLE",
 "entry": [
   {
     "type": {
       "value": "feed"
     },
     "id": "ID",
     "title": "TITLE",
     "summary": "DESCRIPTION",
    "published": "YYYY-MM-DDTHH:mm:ss.sssZ <PUBLISH DATE - ISO8601>",
     "updated": "YYYY-MM-DDTHH:mm:ss.sssZ <UPDATE DATE - ISO8601>",
     "author": {
       "name": "AUTHOR"
     },
     "media_group": [
       {
         "type": "image",
         "media_item": [
           {
             "src": "http://your.link.here.com/ipad/image.jpg",
             "key": "image_1", //Portrait Image
             "type": "image"
           }
           {
             "src": "http://your.link.here.com/ipad/image.jpg",
             "key": "image_base", //Landscape Image
             "type": "image"
           }
         ]
       }
     ],
     "content": {
       "type": "feed",
       "src": "provider://fetchData?type=category&url=URL TO JSON WITH SHOW CONTENT"
     },
     "link": {
       "type": "feed",
       "rel": "self",
       "src": "provider://fetchData?type=category&url=URL TO JSON WITH SHOW CONTENT"
     }
   }
 ]
}

```

# UI Builder Configuration


## Notes

This product should not be thought of as a search engine.

#### **Known issues** 

