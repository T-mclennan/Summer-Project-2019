# Application Folder

## This project was from the summer semester of 2019. We worked as a team of 7 and completed as much as we could in the 8 weeks. 

# GET: /search
request template

    {
      "category" : "{dropdown selection}",
      "neighborhood" : "{dropdown selection}",
      "park_name" : "{dropdown selection}",
      "user_entry" : "{user entered text"}
    }

response template

    [
        {
            "report_id": "test",
            "report_insert_date": "2019-07-14T13:52:50.000Z",
            "report_update_date": null,
            "report_status": "tes",
            "category": "test_category",
            "loc_lat": null,
            "loc_long": null,
            "location_name": "test_location",
            "report_details": "test details",
            "report_user_id": "test_user_id",
            "assigned_to": null,
            "neighborhood": null
        }
    ]

# GET : /reports
request template

    {
        "report_id" : {report_id}
    }
    
 response template

    {
        "report_id": "1563847194954",
        "insert_date": "2019-07-23T09:59:55.000Z",
        "update_date": null,
        "category_id": "1",
        "details": "test_details",
        "status": "unassigned",
        "assigned_to": null,
        "location_id": "1",
        "park_id": "1",
        "image_ref": "test_image",
        "loc_lat": 0,
        "loc_long": 0,
        "user_id": "1"
    }
    
# POST : /reports 
request template

    {
        "category_id" : {dropdown_selection},
        "location_id" : {dropdown_selection},
        "park_id" : {dropdown_selection},
        "details" : {dropdown_selection},
        "loc_lat" : {generated from pin or location selection},
        "loc_long" : {generated from pin or location selection},
        "user_id" : {user_id}
        "image_ref" : {handled in whatever way is easiest to upload image}
    }
  response template

    {
        "fieldCount": {int},
        "affectedRows": {int},
        "insertId": {int},
        "serverStatus": {int},
        "warningCount": {int},
        "message": "",
        "protocol41": true,
        "changedRows": {int},
        "report_id": {report_id}
    }
      
     
