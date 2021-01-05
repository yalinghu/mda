#Reindex - convert the field type of latitude and longitude from string to geo_point

’GET new_311service/_mapping‘

’‘’
PUT new_311service
{
  "mappings": {
    "properties" : {
      "location" : {
        "type" : "geo_point"
      }
    }
  }
}
‘’‘

’‘’
POST _reindex
{
  "source": {
    "index": "311service"
  },
  "dest": {
    "index": "new_311service"
  },
  "script": {
    "source": "ctx._source.location = ['lat': ctx._source.latitude, 'lon': ctx._source.longitude]"
  }
}
‘’‘
