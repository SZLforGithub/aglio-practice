## Create Post [/api/post/]

### Create Post [POST]
create post

+ Request (application/json)
    + Body

            {
                "title": "test",
                "content": "This is a test post."
            }

- Response 200 (application/json)
    - Body

            {
                "id": 1,
                "title": "test",
                "content": "This is a test post.",
                "created_at": "2020/11/11"
            }

## Other Post api [/api/post/{id}]

+ Parameters
    + id: `1` (integer, required) - post id

### Get Post [GET]
get post

- Response 200 (application/json)
    - Body

            {    
                "id": 1,
                "title": "test",
                "content": "This is a test post.",
                "created_at": "2020/11/11" 
            }

### Update Post [PUT]
get post

+ Request (application/json)
    + Body

            {
                "title": "test_updated",
                "content": "This is a test updated post"
            }

- Response 200 (application/json)
    - Body

            {    
                "id": 1,
                "title": "test_updated",
                "content": "This is a test updated post",
                "created_at": "2020/11/11" 
            }

### Delete Post [DELETE]
delete post

- Response 200